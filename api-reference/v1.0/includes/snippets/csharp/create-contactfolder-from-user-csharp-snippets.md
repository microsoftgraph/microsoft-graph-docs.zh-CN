---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a284d21454f9224728d87ec7755ca83653c9b5977f599edd7f9ad1a47b82d2a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    ParentFolderId = "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
    DisplayName = "Important contacts"
};

await graphClient.Me.ContactFolders
    .Request()
    .AddAsync(contactFolder);

```