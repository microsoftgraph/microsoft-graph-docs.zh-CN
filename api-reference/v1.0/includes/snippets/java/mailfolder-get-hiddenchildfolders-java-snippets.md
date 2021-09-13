---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fa872bf578471bc836023e0c9ebc56d77e88825b6d5e32df098131b20cdb343
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("includeHiddenFolders", "true"));

MailFolderCollectionPage childFolders = graphClient.me().mailFolders("{id}").childFolders()
    .buildRequest( requestOptions )
    .get();

```