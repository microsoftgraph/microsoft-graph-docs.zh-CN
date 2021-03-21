---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d766b12ceb92005362b004959f478d725b711a40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977521"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationTemplateCollectionPage applicationTemplates = graphClient.applicationTemplates()
    .buildRequest()
    .get();

```