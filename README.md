// Player Movement Script in Unity (C#)
public class PlayerMovement : MonoBehaviour
{
    public float speed = 10.0f;

    void Update()
    {
        float horizontal = Input.GetAxis("Horizontal") * speed * Time.deltaTime;
        float vertical = Input.GetAxis("Vertical") * speed * Time.deltaTime;
        transform.Translate(horizontal, vertical, 0);
    }
}
