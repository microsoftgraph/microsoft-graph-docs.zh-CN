---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6e0fb1c970cfa80e76c3ea9d6992f5fab993fdfe17ef88af751cfe826c670ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219763"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSynchronizationErrorCollectionPage errors = graphClient.education().synchronizationProfiles("{id}").errors()
    .buildRequest()
    .get();

```