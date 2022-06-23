<template>
  <div class="container" style="max-width: 600px">
    <!-- Heading -->
    <h2 class="text-center mt-5">Todo App</h2>
    <!-- Input -->
    <div class="row">
      <div class="col">
        <div class="card border-1">
          <div class="card-body">
            <form @submit.prevent="submitTask">
              <div class="form-group row mb-2">
                <label for="name" class="col-sm-2 col-form-label">Task Name</label>
                <div class="col-sm-10">
                  <input type="text"  v-model="tasks.name" class="form-control" id="name" placeholder="Task Name">
                </div>
              </div>
              <div class="form-group row mb-2">
                <label for="date" class="col-sm-2 col-form-label">Date</label>
                <div class="col-sm-10">
                  <input type="date"  v-model="tasks.date" class="form-control" id="date">
                </div>
              </div>
              <div class="form-group row mb-2">
                <div class="col-sm-2">Status</div>
                <div class="col-sm-10">
                  <div class="form-check">
                    <input class="form-check-input" v-model="tasks.status"  type="checkbox" id="gridCheck1">
                  </div>
                </div>
              </div>
              <div class="form-group row ">
                <div class="col-sm-10 ">
                  <button type="submit" class="btn btn-primary">Add List</button>
                </div>
              </div>
            </form>
          </div>

        </div>
      </div>
    </div>

    <!-- Task table -->
    <table class="table table-bordered mt-5">
      <thead>
      <tr>
        <th scope="col">Task Name</th>
        <th scope="col" style="width: 140px">Date</th>
        <th scope="col" style="width: 120px">Status</th>
        <th scope="col" class="text-center">#</th>
        <th scope="col" class="text-center">#</th>
      </tr>
      </thead>
      <tbody>
      <tr>
        <td>
          hello
        </td>
        <td>
          23/06/22
        </td>
        <td class="text-center">
        </td>
        <td class="text-center">
        </td>
      </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'TodoList',
  data(){
    return {
        tasks:{
          name:'',
          date:'',
          status:''
        }
    }
  },
  methods:{
    submitTask(){

    }
  }
}
</script>

<style scoped>

</style>
