---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97db53acb30c7289186089511fe2602a9a9d8d33
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367237"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage search = graphClient.me().drive().root()
    .search("{search-query}")
    .buildRequest()
    .get();

```