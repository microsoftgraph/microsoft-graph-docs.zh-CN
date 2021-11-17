---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d5155c57fb7fdb49a45c0542d02ee91028d5c80a9942829496cc39f588ddd94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("format", "{format}"));

InputStream stream = graphClient.customRequest("/drive/items/{item-id}/content", InputStream.class)
    .buildRequest( requestOptions )
    .get();

```