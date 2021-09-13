---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcd071b95572e7e8cfc730c2dd1d4d5ab2977703ce4e3ebf8f264297bbeb7b4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158697"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .buildRequest()
    .delete();

```