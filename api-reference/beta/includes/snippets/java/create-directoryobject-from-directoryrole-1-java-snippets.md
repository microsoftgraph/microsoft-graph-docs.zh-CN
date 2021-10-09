---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46b0d794f36e9227bbe5765863901d3991c101ba00bfa087caa440dc9c1b37ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105227"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "0f933635-5b77-4cf4-a577-f78a5eb090a2";

graphClient.directoryRoles("0afed502-2456-4fd4-988e-3c21924c28a7").members().references()
    .buildRequest()
    .post(directoryObject);

```