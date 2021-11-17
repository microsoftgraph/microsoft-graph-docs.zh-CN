---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7eaa9b0cc739ef6d67a0e8889285d1d4ef5c947c8a144173d7054eb4e521f73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219023"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolderCollectionPage childFolders = graphClient.me().mailFolders("AAMkAGVmMDEzM").childFolders()
    .buildRequest()
    .get();

```