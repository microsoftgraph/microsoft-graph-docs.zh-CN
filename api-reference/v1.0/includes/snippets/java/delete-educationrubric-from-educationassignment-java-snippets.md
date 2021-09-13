---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbfdf4ae0aa632b6a9bb7de8ffa7a05d08b8d6c16345073ea3231095b0d84300
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").rubric().reference()
    .buildRequest()
    .delete();

```