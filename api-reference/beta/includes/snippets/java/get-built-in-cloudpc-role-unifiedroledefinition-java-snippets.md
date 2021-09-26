---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ddd0eb896ba27d97dcfa875697ed7336e9cf60297b568b96cec8a51ab7d9139
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinition unifiedRoleDefinition = graphClient.roleManagement().cloudPC().roleDefinitions("d40368cb-fbf4-4965-bbc1-f17b3a78e510")
    .buildRequest()
    .get();

```