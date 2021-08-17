---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c18c3416cda63cddad2744ea54d44032f2e19c85c010f95a589f77ce514b359c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const certificateBasedAuthConfiguration = {
  certificateAuthorities: [
    {
      isRootAuthority: true,
      certificate: 'Binary'
    }
  ]
};

await client.api('/organization/{id}/certificateBasedAuthConfiguration/$ref')
    .post(certificateBasedAuthConfiguration);

```