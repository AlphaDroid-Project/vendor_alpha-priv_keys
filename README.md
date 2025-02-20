# alpha-priv_keys-template

# Usage

```bash
git clone https://github.com/alphadroid-project/vendor_alpha-priv_keys vendor/alpha-priv/keys
```

```bash
cd vendor/alpha-priv/keys
```

```
./keys.sh
```

# Testing

Included `check_keys.py` script checks whether all apk/apex/capex files in the build out are signed with keys within its directory. Be aware that some targets are **expected** to be signed with vendor key, for example `com.android.apex.cts.shim.v1_prebuilt`.

```
$ ./check_keys.py ~/alpha/out/target/product/grus
/home/ab/alpha/out/target/product/grus/obj/ETC/com.android.apex.cts.shim.v1_prebuilt_intermediates/com.android.apex.cts.shim.apex is signed with an unknown key!
```
