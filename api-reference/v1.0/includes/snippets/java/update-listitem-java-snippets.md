---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b24cde1368eef867540ae1b4829a780ad4d8243b77f0c5d16dc43ca976bed406
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104326"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FieldValueSet fieldValueSet = new FieldValueSet();
fieldValueSet.Color = "Fuchsia";
fieldValueSet.Quantity = 934;

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").fields()
    .buildRequest()
    .patch(fieldValueSet);

```