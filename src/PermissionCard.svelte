<script>

</script>

<div class="permisstionCard">
    <h2>
        <slot name="sysPermisstionType">
            <span class="missing">
                unknown name
        </slot>
    </h2>

    <div class="queryAll">
        <slot name="queryPermission">
            <span class="missing">
                unknown function
            </span>
        </slot>    
    </div>

    <div>
        <slot name="editAll">
            <span class="missing">
                unknown function
            </span>
        </slot>      
    </div>

    <div>
        <slot name="addAll">
            <span class="missing">
                unknown function
            </span>
        </slot>      
    </div>

    <div>
        <slot name="delAll">
            <span class="missing">
                unknown function
            </span>
        </slot>        
    </div>
</div>

<style>
    .permisstionCard {
		width: 250px;
		border: 1px solid #aaa;
		border-radius: 2px;
		box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
		padding: 1em;        
    }

    h2 {
		padding: 0 0 0.2em 0;
		margin: 0 0 1em 0;
		border-bottom: 1px solid #ff3e00
	}

    .missing { color: #999 }
</style>