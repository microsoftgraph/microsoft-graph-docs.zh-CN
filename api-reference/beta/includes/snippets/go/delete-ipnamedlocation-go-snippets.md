---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d06c7600ac4baca355a8f148c849ec05c958a9a4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981419"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

namedLocationId := "namedLocation-id"
graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Delete(options)


```