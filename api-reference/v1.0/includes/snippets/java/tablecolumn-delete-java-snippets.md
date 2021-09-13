---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e78d0f21d5fba21932668831ff500d18d1fd31e4e929539a6af661291e4a608
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328734"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .buildRequest()
    .delete();

```