---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcd72ef38bb485f67db7f0cab7c10552bb59b9c9e9bd0038bfdc939055b671c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161369"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = graphClient.teams("{id}").primaryChannel()
    .buildRequest()
    .get();

```