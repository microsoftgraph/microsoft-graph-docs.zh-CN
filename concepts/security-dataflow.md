---
title: Microsoft Graph 安全 API 数据流
description: Microsoft Graph 安全 API 建立联盟与 Microsoft Graph Security 生态系统中的所有提供商的请求。 这基于应用程序，提供安全提供程序同意，如下图中所示。 同意工作流仅适用于非 Microsoft 提供程序。
ms.openlocfilehash: 1e8b074e3cf4589ca67364ed7e225a62f40300fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091845"
---
# <a name="microsoft-graph-security-api-data-flow"></a>Microsoft Graph 安全 API 数据流

Microsoft Graph 安全 API 建立联盟与 Microsoft Graph Security 生态系统中的所有提供商的请求。 这基于应用程序，提供安全提供程序同意，如下图中所示。 同意工作流仅适用于非 Microsoft 提供程序。

![security_dataflow_1.png](./images/security-dataflow-1.png)

以下是流的说明：

1. 应用程序用户登录到要查看从提供程序的同意窗体的提供程序应用程序。 此窗体的同意体验或 UI 由提供程序，适用于非 Microsoft 提供程序仅要从其客户将请求发送到 Microsoft Graph 安全 API 获取明确同意。
2. 客户端同意存储提供程序侧。
3. 提供程序 consent 服务调用 Microsoft Graph 安全 API，告知各自的客户的同意审批。
4. 应用程序将请求发送到 Microsoft Graph 安全 API。
5. Microsoft Graph 安全 API 检查此客户映射到不同的提供程序的许可信息。
6. Microsoft Graph 安全 API 调用所有客户提供了通过提供程序同意体验的明确同意这些提供程序。
7. 从该客户端的 consented 提供程序返回的响应。
8. 结果集响应返回到应用程序。
9. 如果客户已不同意任何提供程序，在响应中不包含这些提供程序的任何结果。
