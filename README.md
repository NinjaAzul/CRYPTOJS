# CRYPTOJS

```ts
import * as CryptoJS from 'crypto-js';

export const encrypt = (text: string): string => {
  return CryptoJS.AES.encrypt(text, process.env.ENCRYPT_KEY).toString();
};

export const decrypt = (text: string): string => {
  const bytes = CryptoJS.AES.decrypt(text, process.env.ENCRYPT_KEY);
  return bytes.toString(CryptoJS.enc.Utf8);
};


```
