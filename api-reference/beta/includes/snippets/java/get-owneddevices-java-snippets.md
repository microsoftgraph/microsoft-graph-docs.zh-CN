---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cfdbc98dcd4dc63a03d0b822184f9a12ebe5c5e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979833"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage ownedDevices = graphClient.me().ownedDevices()
    .buildRequest()
    .get();

```