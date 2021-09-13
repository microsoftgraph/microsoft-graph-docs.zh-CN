---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f57478b3afa0ae11bf4a6824eff7aab64d6203f5b6977609ecce171746b28ba0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107019"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UsedInsightCollectionPage used = graphClient.me().insights().used()
    .buildRequest()
    .orderBy("LastUsed/LastAccessedDateTime desc")
    .get();

```