---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b95c94ed6ce9f87d7b3a03bbd88213c42851dad363577a7d535db616c6f74e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277302"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolderCollectionPage taskFolders = graphClient.me().outlook().taskFolders()
    .buildRequest()
    .get();

```