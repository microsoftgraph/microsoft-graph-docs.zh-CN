---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaff7d196f3cea2cb8f3841800bc8c5db85a90e2da9cf6ec2d0fc0ad52db9bc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
  delegateMeetingMessageDeliveryOptions: "sendToDelegateAndPrincipal"
};

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings')
    .version('beta')
    .update(mailboxSettings);

```