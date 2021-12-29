class LoginFragment : Fragment()
override fun onCreateView(
        inflater: LayoutInflater,
        container: ViewGroup?,
        savedInstanceState: Bundle?
): View? {
    return inflater.inflate(R.layout.login_fragment, container, false)
}
override fun onViewCreated(view: View, savedInstanceState: Bundle?) {
    super.onViewCreated(view, savedInstanceState)
}
class LoginFragment : Fragment() {

    private lateinit var usernameEditText: EditText
    private lateinit var passwordEditText: EditText
    private lateinit var loginButton: Button
    private lateinit var statusTextView: TextView

    override fun onViewCreated(view: View, savedInstanceState: Bundle?) {
        super.onViewCreated(view, savedInstanceState)

        usernameEditText = view.findViewById(R.id.username_edit_text)
        passwordEditText = view.findViewById(R.id.password_edit_text)
        loginButton = view.findViewById(R.id.login_button)
        statusTextView = view.findViewById(R.id.status_text_view)
    }

    ...
}
loginButton.setOnClickListener {
    val authSuccessful: Boolean = viewModel.authenticate(
            usernameEditText.text.toString(),
            passwordEditText.text.toString()
    )
    if (authSuccessful) {
        // Navigate to next screen
    } else {
        statusTextView.text = requireContext().getString(R.string.auth_failed)
    }
}
class LoginFragment : Fragment() {

    ...

    companion object {
        private const val TAG = "LoginFragment"
    }
}
private val viewModel: LoginViewModel by viewModels()
val name: String = null
val name: String? = null
public class Account implements Parcelable {
    public final String name;
    public final String type;
    private final @Nullable String accessId;

    ...
}
public class Account implements Parcelable {
    public final @NonNull String name;
    ...
}
val account = Account("name", "type")
val accountName = account.name!!.trim()
val account = Account("name", "type")
val accountName = account.name?.trim()
val account = Account("name", "type")
val accountName = account.name?.trim() ?: "Default name"
fun validateAccount(account: Account?) {
    val accountName = account?.name?.trim() ?: "Default name"

    // account cannot be null beyond this point
    account ?: return

    ...
}
class LoginFragment : Fragment() {
    val index: Int = 12
}
class LoginFragment : Fragment() {
    val index: Int

    init {
        index = 12
    }
}
class LoginFragment : Fragment() {
    private var statusTextView: TextView? = null

    override fun onViewCreated(view: View, savedInstanceState: Bundle?) {
            super.onViewCreated(view, savedInstanceState)

            statusTextView = view.findViewById(R.id.status_text_view)
            statusTextView?.setText(R.string.auth_failed)
    }
}
class LoginFragment : Fragment() {
    private lateinit var statusTextView: TextView

    override fun onViewCreated(view: View, savedInstanceState: Bundle?) {
            super.onViewCreated(view, savedInstanceState)

            statusTextView = view.findViewById(R.id.status_text_view)
            statusTextView.setText(R.string.auth_failed)
    }
}
