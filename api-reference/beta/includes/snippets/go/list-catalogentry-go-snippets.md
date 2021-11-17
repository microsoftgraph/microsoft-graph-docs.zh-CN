---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c09a28fd7d9c66a9d3dab504041ce58a0f7e495
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029959"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Admin().Windows().Updates().Catalog().Entries().Get(options)


```