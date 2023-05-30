<script>
export let text;
export let type;
</script>

<button class={type}>{text}</button>

<style lang="scss">
button {
    font-size: 14px;
    padding: 6px 12px;
    border: none;
    outline: none;
    border-radius: 3px;
    box-sizing: border-box;
    cursor: pointer;
    display: inline-flex;
    font-weight: 400;
    justify-content: center;
    line-height: 1.4;
    position: relative;
    transition: all .3s ease-in-out;
    -webkit-user-select: none;
    -ms-user-select: none;
    user-select: none;

    &:focus-visible {
        box-shadow: 0 0 0 2px #fff, 0 0 0 4px #10a37f;
    }
}

.primary {
    color: #fff;
    background-color: #10a37f;

    &:active {
        background-color: #1b5d4a;
    }

    &:hover {
        background-color: #1a7f64;
    }

    &:focus {
        box-shadow: 0 0 0 3px rgba(16,163,127,.3);
    }
}

.secondary {
    background-color: #ececf1;
    color: #353740;

    &:active {
        background-color: #c5c5d2;
    }

    &:hover {
        background-color: #d9d9e3;
    }

    &:focus {
        box-shadow: 0 0 0 3px rgba(217, 217, 227, .3);
    }
}
</style>