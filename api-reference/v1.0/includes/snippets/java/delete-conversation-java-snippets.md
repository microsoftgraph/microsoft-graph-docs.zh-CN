---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbf1936fa87201135fb1fe092a7cf7813f0712beac2b11d009d17978dbbda3f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221014"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").conversations("{id}")
    .buildRequest()
    .delete();

```