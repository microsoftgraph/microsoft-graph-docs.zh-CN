---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32edf4eb853748d9b4a204b567dac1498e47b881
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982294"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleTemplateCollectionPage directoryRoleTemplates = graphClient.directoryRoleTemplates()
    .buildRequest()
    .get();

```