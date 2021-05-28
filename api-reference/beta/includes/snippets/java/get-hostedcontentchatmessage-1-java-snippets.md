---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58e7b29ea1b9024dac67175ebba39475adc42a76
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610036"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContent chatMessageHostedContent = graphClient.chats("19:2da4c29f6d7041eca70b638b43d45437@thread.v2").messages("1615971548136").hostedContents("aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv")
    .buildRequest()
    .get();

```