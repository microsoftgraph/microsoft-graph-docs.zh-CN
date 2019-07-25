---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 27480439678af338071374f883eea816100c3d94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861193"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("format", "{format}"));

Stream Stream = graphClient.customRequest("/drive/items/{item-id}/content", Stream.class)
    .buildRequest( requestOptions )
    .get();

```