---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fadd62df886c34965d6802323e9aed5c6b888aec
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951495"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers("006111db-0810-4494-a6df-904d368bd81b")
    .buildRequest()
    .delete();

```