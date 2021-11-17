---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abcbf387d50f5e175ed8835f703cb9f07664aed0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976166"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamsAppId := "teamsApp-id"
graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).Delete(options)


```