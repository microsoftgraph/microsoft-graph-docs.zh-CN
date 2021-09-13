---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4f4fc7c62156d5900046b1f31638d7c213f4d34eec3a59a80521c8644952488
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219814"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  parentFolderId: 'AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==',
  displayName: 'Important contacts'
};

await client.api('/me/contactFolders')
    .post(contactFolder);

```