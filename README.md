# shhhinterrupt

Gracefully and silently handle keyboard interrupts.

You can either pass a string to print, e.g. `@handle_interrupt("Please come again.")` or you can use the decorator without parenthesis to use the default message `@handle_interrupt`.

Full example:

    from shhhinterrupt import handle_interupt
    import time
    
    @handle_interrupt("He walked away.")
    def main():
        print("What's your name?")
        time.sleep(5)
        print("Tony!")

    if __name__ == "main":
        main()
