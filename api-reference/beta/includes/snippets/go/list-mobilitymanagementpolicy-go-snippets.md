---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 141ca70c0e22b49f9292a134f4d4b0ea5b09eeaf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086044"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().MobileDeviceManagementPolicies().Get(options)


```