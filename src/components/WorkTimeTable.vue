<template>
  <table class="is-small" style="width: 100%">
    <thead>
      <tr>
        <th>
          <p>День</p>
        </th>
        <th>
          <p>Время</p>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          <p>Понедельник</p>
        </td>
        <td>
          <p>Выходной</p>
        </td>
      </tr>
      <tr>
        <td>
          <p>Вторник</p>
        </td>
        <td>
          <p>10:00 — 17:00</p>
        </td>
      </tr>
      <tr>
        <td>
          <p>Среда</p>
        </td>
        <td>
          <p>10:00 — 17:00</p>
        </td>
      </tr>
      <tr>
        <td>
          <p>Четверг</p>
        </td>
        <td>
          <p>10:00 — 17:00</p>
        </td>
      </tr>
      <tr>
        <td>
          <p>Пятница</p>
        </td>
        <td>
          <p>10:00 — 17:00</p>
        </td>
      </tr>
      <tr>
        <td>
          <p>Суббота</p>
        </td>
        <td>
          <p>10:00 — 17:00</p>
        </td>
      </tr>
      <tr>
        <td>
          <p>Воскресенье</p>
        </td>
        <td>
          <p>10:00 — 17:00</p>
        </td>
      </tr>
    </tbody>
  </table>
</template>

<style scoped>
@reference '../assets/main.css';

th,
td {
  @apply text-left p-2 text-accent border-b-line border-b-2
}

p {
  @apply text-base
}

th {
  @apply border-b-2
}
</style>