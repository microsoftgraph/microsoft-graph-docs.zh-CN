---
author: besiler
ms.topic: include
ms.date: 05/11/2022
ms.localizationpriority: medium
ms.openlocfilehash: 051f4e0cd02e2e55219bf977e36c74098296c773
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971867"
---
<!-- markdownlint-disable MD041-->

### <a name="viewing-applied-conditional-access-ca-policies-in-sign-ins"></a>在登录中查看应用的条件访问 (CA) 策略
**appliedConditionalAccessPolicies** 属性中列出的已应用 CA 策略仅适用于具有允许他们读取 [条件访问数据](/graph/api/resources/appliedconditionalaccesspolicy)的角色的用户和应用。 如果用户或应用有权读取登录日志，但无权读取条件访问数据，则将省略响应中的 **appliedConditionalAccessPolicies** 属性。 以下 Azure AD 角色授予用户查看条件访问数据的权限：

+ 全局管理员
+ 全局读取者
+ 安全管理员
+ 安全读取者
+ 条件访问管理

应用程序必须至少具有以下权限之一才能在登录日志中查看 [appliedConditionalAccessPolicy](/graph/api/resources/appliedconditionalaccesspolicy) 对象： 

+ Policy.Read.All
+ Policy.ReadWrite.ConditionalAccess
+ Policy.Read.ConditionalAccess

>**注意：** 具有任何权限的 Azure AD 用户可以读取登录日志，其中用户是登录的执行组件。 此功能可帮助用户发现其帐户中的意外活动。 用户无法从自己的日志中读取 CA 数据，除非他们具有上面标识的 CA 权限之一。
