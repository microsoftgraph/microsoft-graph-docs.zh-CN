---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 278858d2b216175ca25dd69ecf79edbdf030598a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Security().TiIndicators().SubmitTiIndicators().Post(options)


```