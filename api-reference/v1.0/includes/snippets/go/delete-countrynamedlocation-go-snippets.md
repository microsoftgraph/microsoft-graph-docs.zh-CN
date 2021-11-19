---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f1f1bd8221cfdf5b26a8acf5a05bf69f0405b97
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082601"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

namedLocationId := "namedLocation-id"
graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Delete(options)


```