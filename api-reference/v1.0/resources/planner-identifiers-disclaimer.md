---
title: Planner 中的标识符
description: 'Planner 中的对象标识符是由服务生成的字符串值。 这些值的长度为28个字符, 区分大小写。 当作为 in 传递时, 服务将对标识符进行简单的格式验证, 如果格式验证失败, 调用方将收到指示此问题的错误请求 (400) 错误响应。 如果收到此错误, 则表示调用应用程序中有一个错误, 如:'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 75a0262b085b6649d7390a2a6196d0190cdefc5d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035446"
---
# <a name="identifiers-in-planner"></a>Planner 中的标识符

Planner 中的对象标识符是由服务生成的字符串值。 这些值的长度为28个字符, 区分大小写。 当作为 in 传递时, 服务将对标识符进行简单的格式验证, 如果格式验证失败, 调用方将收到指示此问题的错误请求 (400) 错误响应。 如果收到此错误, 则表示调用应用程序中有一个错误, 如:

- 调用应用程序将标识符处理为不区分大小写的字符串。 任务中的标识符区分大小写。
- 调用应用程序截断了标识符。 任务中的标识符长度为28个字符。
- 调用应用程序尝试为任务中的对象生成标识符值。 不接受客户端生成的标识符。 所有标识符都是在创建对象时由服务生成的。

此验证**不是一项安全功能**。 它仅用于在开发应用程序期间通知应用程序与常见标识符相关的问题, 这些问题在其他方面很难识别。
