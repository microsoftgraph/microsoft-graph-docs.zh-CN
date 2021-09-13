---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbe4b7c3fbf7d768849de0e34faca1c45370a0f7973485399a2ff0042f70345b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage users = graphClient.education().schools("{school-id}").users()
    .buildRequest()
    .get();

```