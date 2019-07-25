---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb6ba3551451b24e4d42e184c53392ded85991d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880697"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields"));

ListItem listItem = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
    .buildRequest( requestOptions )
    .get();

```