---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: faa57a7aa00edcc5252808cc278fc0c651bee7a79cf5669bc2ba138b8d3adf93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163105"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTriggerCollectionPage taskTriggers = graphClient.print().printers("{id}").taskTriggers()
    .buildRequest()
    .get();

```