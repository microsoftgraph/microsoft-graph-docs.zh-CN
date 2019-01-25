---
title: 任务中的标识符
description: 任务中对象的标识符是服务生成的字符串值。 . 值 28 字符，都区分大小写。 作为中传递，该服务将执行操作标识符，简单格式的验证，如果格式验证失败，呼叫者将收到错误请求 (400) 错误响应，指示此问题。 收到此错误指示 bug 中调用应用程序，如：
localization_priority: Normal
ms.openlocfilehash: 98a999fa2473a8f77b316d6acf668aec9c3ac832
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527610"
---
# <a name="identifiers-in-tasks"></a>任务中的标识符

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

任务中对象的标识符是服务生成的字符串值。 . 值 28 字符，都区分大小写。 作为中传递，该服务将执行操作标识符，简单格式的验证，如果格式验证失败，呼叫者将收到错误请求 (400) 错误响应，指示此问题。 收到此错误指示 bug 中调用应用程序，如：

- 调用应用程序将此标识符处理为不区分大小写的字符串。任务中的标识符区分大小写。
- 调用应用程序截断了该标识符。任务中的标识符长度为 28 个字符。
- 调用应用程序尝试为任务中的对象生成标识符值。不接受客户端生成的标识符。所有标识符均在创建对象后由服务生成。

此验证**不是安全功能**。它仅用于告知应用程序关于应用程序开发期间常见的标识符相关问题的信息，如果不告知这些信息则很难标识这些问题。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/tasks-identifiers-disclaimer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
