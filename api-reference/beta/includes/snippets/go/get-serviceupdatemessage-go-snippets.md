---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acb3498485a76e2b299199ede5512a292cf65d59
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085773"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceUpdateMessageId := "serviceUpdateMessage-id"
result, err := graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).Get(options)


```