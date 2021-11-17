---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d01718f25dbf2410ac5504aad7fef6e4af30e300
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023454"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupSettingId := "groupSetting-id"
result, err := graphClient.GroupSettingsById(&groupSettingId).Get(options)


```