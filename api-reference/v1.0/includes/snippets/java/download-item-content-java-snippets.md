---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eadcc990a1a32bad99d5c7a8da0e9e77bb6cf2e9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890939"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream Stream = graphClient.customRequest("/me/drive/items/{item-id}/content", Stream.class)
    .buildRequest()
    .get();

```