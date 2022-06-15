---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b18dad9c40b166f62b5cd54919cedeb9563952d5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092141"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryNoncustodialDataSource ediscoveryNoncustodialDataSource = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").noncustodialDataSources("35393639323133394345384344303043")
    .buildRequest()
    .expand("dataSource")
    .get();

```