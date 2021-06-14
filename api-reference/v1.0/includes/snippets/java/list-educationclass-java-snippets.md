---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 655ba97e2735096988031d4478ad0474e8bae81a
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871334"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage taughtClasses = graphClient.education().users("{educationUserId}").taughtClasses()
    .buildRequest()
    .get();

```