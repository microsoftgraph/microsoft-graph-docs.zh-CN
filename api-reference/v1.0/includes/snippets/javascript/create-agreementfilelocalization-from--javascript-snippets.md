---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cbfc164ef05e69123f9719a4c7c527cfbbe473e
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreementFileLocalization = {
    fileName: 'Contoso ToU for guest users (French)',
    language: 'fr-FR',
    isDefault: false,
    isMajorVersion: false,
    displayName: 'Contoso ToU for guest users (French)',
    fileData: {
        data: 'base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data'
    }
};

await client.api('/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/files')
    .post(agreementFileLocalization);

```