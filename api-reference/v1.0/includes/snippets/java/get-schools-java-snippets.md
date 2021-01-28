---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf5704afbc7307e51ed51881540d8941bf74f3dd
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015251"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSchoolCollectionWithReferencesPage schools = graphClient.education().classes("{class-id}").schools()
    .buildRequest()
    .get();

```