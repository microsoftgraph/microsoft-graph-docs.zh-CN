---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c3084e62fa4f4d1ef056bef103c330fbf8c8382b483d0f9861548be20c0739b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219815"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.parentFolderId = "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==";
contactFolder.displayName = "Important contacts";

graphClient.me().contactFolders()
    .buildRequest()
    .post(contactFolder);

```