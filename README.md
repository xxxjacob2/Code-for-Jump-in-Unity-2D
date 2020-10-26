public Rigidbody2D rb;

Public float jumpForce;
// dont need a void start
void Update()
{
    if (Input.GetKeyDown(KeyCode.Space))
    {
        Jump();
    }
}

void Jump()
{
    rb.velocity = Vector2.up * jumpForce;
}
