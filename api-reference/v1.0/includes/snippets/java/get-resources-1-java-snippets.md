---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f4f1ad439bb705b240966801ba7959dfd24c7633ebede4f7a32e74567e4ced1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409576"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResourceCollectionPage resources = graphClient.education().classes("d38ffdea-da93-46ac-90ba-d568c6073075").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").resources()
    .buildRequest()
    .get();

```