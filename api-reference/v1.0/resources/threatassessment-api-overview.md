---
title: 使用 Microsoft Graph 威胁评估 API
description: 通过 Microsoft Graph，你的应用可获得授权访问组织的威胁评估数据。
localization_priority: Priority
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 0837dae4482174bb8ccab05791c61dfb17eb6c80d6e1cdc3337cdfddb6d1636b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124022"
---
# <a name="use-the-microsoft-graph-threat-assessment-api"></a>使用 Microsoft Graph 威胁评估 API

Microsoft Graph 威胁评估 API 可帮助组织评估租户中任何用户收到的威胁。 这样，客户就可将其收到的垃圾电子邮件、网络钓鱼 URL 或恶意软件附件报告给 Microsoft。 策略检查结果和重新扫描结果可帮助租户管理员了解威胁扫描判定并调整其组织策略。

## <a name="authorization"></a>Authorization

Microsoft Graph 通过权限控制对资源的访问。 必须指定访问威胁评估资源所需的权限。 通常是在 Azure Active Directory (Azure AD) 门户中指定权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[威胁评估权限](/graph/permissions-reference#threat-assessment-permissions)。

## <a name="common-use-cases"></a>常见用例

Microsoft Graph 威胁评估 API 提供了用来列出、创建和获取威胁评估请求以及检索评估结果的方法。

| 用例 | REST 资源 | 另请参阅 |
|:----------|:---------------|:---------|
| 列出、创建和获取威胁评估请求 | [threatAssessmentRequest](../resources/threatassessmentrequest.md)<br> [mailAssessmentRequest](../resources/mailAssessmentRequest.md)<br> [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)<br> [fileAssessmentRequest](../resources/fileAssessmentRequest.md)<br> [urlAssessmentRequest](../resources/urlAssessmentRequest.md)<br> | [创建 threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md)<br> [获取 threatAssessmentRequest](../api/threatassessmentrequest-get.md)<br> [列出 threatAssessmentRequest](../api/informationprotection-list-threatassessmentrequests.md) |
| 获取威胁评估结果 | [threatAssessmentResult](../resources/threatassessmentresult.md) | [获取 threatAssessmentResult](../api/threatassessmentrequest-get.md#example-5-expand-threat-assessment-results-for-a-request)|

## <a name="next-steps"></a>后续步骤

威胁评估资源和 API 提供了使用 Microsoft Graph 与用户交互及管理用户体验的新方式。若要了解详细信息：

- 向下钻取[威胁评估请求](../resources/threatassessmentrequest.md)和[威胁评估结果](../resources/threatAssessmentResult.md)资源的[方法](../resources/threatassessmentrequest.md#methods)、[属性](../resources/threatassessmentrequest.md#properties)和[关系](../resources/threatassessmentrequest.md#relationships)。
- 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。


