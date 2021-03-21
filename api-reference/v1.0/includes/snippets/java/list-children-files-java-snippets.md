---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9599033d9ad6b3537b082b6daecdda271d43488d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972615"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage children = graphClient.drives("{drive-id}").items("{item-id}").children()
    .buildRequest()
    .get();

```