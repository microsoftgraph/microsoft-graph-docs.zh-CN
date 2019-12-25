---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6ceb2ad719c34e0e937d490b9e6fb723ce26998
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865797"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "VideoTeleconferenceId eq '123456789'"));

IOnlineMeetingCollectionPage onlineMeetings = graphClient.communications().onlineMeetings()
    .buildRequest( requestOptions )
    .get();

```