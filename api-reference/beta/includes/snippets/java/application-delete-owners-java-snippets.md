---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb275f7c38e93a93e911f0bd4a83303de86ed2515c066ccce66077dd32e88cc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215677"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}").owners("{id}").reference()
    .buildRequest()
    .delete();

```