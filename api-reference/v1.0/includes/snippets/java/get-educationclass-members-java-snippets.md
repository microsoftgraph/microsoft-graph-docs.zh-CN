---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85f87be656040b39c1f16f82ad00215664e81ef9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969044"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage members = graphClient.education().classes("{class-id}").members()
    .buildRequest()
    .get();

```