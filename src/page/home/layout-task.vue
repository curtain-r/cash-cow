<script setup lang="ts">import { reactive } from 'vue';
import { TaskList } from '../../common/const';

    const taskList = reactive<TaskList[]>([]);
</script>
<template>
    <div>taskTitle</div>
    <div class="task-list">
        <div v-for="task of taskList" :key="task.title">
        
        </div>
    </div>
</template>