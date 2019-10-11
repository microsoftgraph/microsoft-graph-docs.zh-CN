---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61dcc2a649c3a9649f4166446366a68b62a4512a
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428841"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("format", "{format}"));

Stream stream = graphClient.customRequest("/me/drive/items/{item-id}/content", Stream.class)
    .buildRequest( requestOptions )
    .get();

```