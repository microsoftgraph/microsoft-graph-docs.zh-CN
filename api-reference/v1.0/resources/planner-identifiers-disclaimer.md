---
title: Planner 中的标识符
description: 计划工具中对象的标识符是服务生成的字符串值。 值 28 字符，都区分大小写。 作为中传递，该服务将执行操作标识符，简单格式的验证，如果格式验证失败，呼叫者将收到错误请求 (400) 错误响应，指示此问题。 收到此错误指示 bug 中调用应用程序，如：
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75c284d576ed6f03691828309fab7ed899c1c066
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951855"
---
# <a name="identifiers-in-planner"></a>Planner 中的标识符

计划工具中对象的标识符是服务生成的字符串值。 值 28 字符，都区分大小写。 作为中传递，该服务将执行操作标识符，简单格式的验证，如果格式验证失败，呼叫者将收到错误请求 (400) 错误响应，指示此问题。 收到此错误指示 bug 中调用应用程序，如：

- 调用应用程序将此标识符处理为不区分大小写的字符串。任务中的标识符区分大小写。
- 调用应用程序截断了该标识符。任务中的标识符长度为 28 个字符。
- 调用应用程序尝试为任务中的对象生成标识符值。不接受客户端生成的标识符。所有标识符均在创建对象后由服务生成。

此验证**不是安全功能**。它仅用于告知应用程序关于应用程序开发期间常见的标识符相关问题的信息，如果不告知这些信息则很难标识这些问题。
