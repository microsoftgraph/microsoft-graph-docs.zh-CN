---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf9a4d038ac3b0544faaf24f40daf8b8c99d068e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970677"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage children = graphClient.me().drive().root().children()
    .buildRequest()
    .get();

```