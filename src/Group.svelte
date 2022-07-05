<script>
  export let width = 128;
  export let height = 128;

  // export let groupName = '範例:系統管理員';
  // export let groupFunctions = '功能項目:Functions';

  const gp = 'group';
</script>

<div class="board">
  <div class='titlePic'>
    <svg width="{width}px" height="{height}px" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg" >
      <title>group</title>
      <path d="M144 288Q104 288 76 260 48 232 48 192 48 152 76 124 104 96 144 96 184 96 212 124 240 152 240 192 240 232 212 260 184 288 144 288ZM368 288Q328 288 300 260 272 232 272 192 272 152 300 124 328 96 368 96 408 96 436 124 464 152 464 192 464 232 436 260 408 288 368 288ZM48 385Q48 357 67 339 85 320 113 320L175 320Q203 320 222 339 240 357 240 385L240 416 48 416 48 385ZM272 385Q272 357 291 339 309 320 337 320L399 320Q427 320 446 339 464 357 464 385L464 416 272 416 272 385Z" />
    </svg>
  </div>

  <div>
    <div class="{gp}Name">
      <h2>
        <slot name="name">
          <span class="missing">Unknown name</span>
        </slot>  
      </h2>
    </div>

    <div class="{gp}Function">
      <slot name="function">
        <span class="missing">Unknown function</span>
      </slot>  
    </div>
  </div>
</div>

<style>
  .board {
    display: flex;
  }
  .groupName {
    margin-top: 15px;
    margin-left: 15px;
  }
  .groupFunction {
    margin-top: 15px;
    margin-left: 15px;    
  }
</style>