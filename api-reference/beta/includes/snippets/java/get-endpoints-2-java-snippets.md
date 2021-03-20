---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2a7ff0f75cce845ae066a85d5d6faaa60f95fab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961479"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintServiceEndpointCollectionPage endpoints = graphClient.print().services("{id}").endpoints()
    .buildRequest()
    .get();

```