---
title: 使用 Microsoft Graph 威胁评估 API
description: 通过 Microsoft Graph，你的应用可获得授权访问组织的威胁评估数据。
localization_priority: Priority
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: aa13befe855fab8094107cee13eae28efff3e4b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090898"
---
# <a name="use-the-microsoft-graph-threat-assessment-api"></a><span data-ttu-id="e2529-103">使用 Microsoft Graph 威胁评估 API</span><span class="sxs-lookup"><span data-stu-id="e2529-103">Use the Microsoft Graph threat assessment API</span></span>

<span data-ttu-id="e2529-104">Microsoft Graph 威胁评估 API 可帮助组织评估租户中任何用户收到的威胁。</span><span class="sxs-lookup"><span data-stu-id="e2529-104">The Microsoft Graph threat assessment API helps organizations to assess the threat received by any user in a tenant.</span></span> <span data-ttu-id="e2529-105">这样，客户就可将其收到的垃圾电子邮件、网络钓鱼 URL 或恶意软件附件报告给 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="e2529-105">This empowers customers to report spam emails, phishing URLs or malware attachments they receive to Microsoft.</span></span> <span data-ttu-id="e2529-106">策略检查结果和重新扫描结果可帮助租户管理员了解威胁扫描判定并调整其组织策略。</span><span class="sxs-lookup"><span data-stu-id="e2529-106">The policy check result and rescan result can help tenant administrators understand the threat scanning verdict and adjust their organizational policy.</span></span>

## <a name="authorization"></a><span data-ttu-id="e2529-107">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2529-107">Authorization</span></span>

<span data-ttu-id="e2529-108">Microsoft Graph 通过权限控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="e2529-108">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="e2529-109">必须指定访问威胁评估资源所需的权限。</span><span class="sxs-lookup"><span data-stu-id="e2529-109">You must specify the permissions you need in order to access threat assessment resources.</span></span> <span data-ttu-id="e2529-110">通常是在 Azure Active Directory (Azure AD) 门户中指定权限。</span><span class="sxs-lookup"><span data-stu-id="e2529-110">Typically, you specify permissions in the Azure Active Directory (Azure AD) portal.</span></span> <span data-ttu-id="e2529-111">有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[威胁评估权限](/graph/permissions-reference#threat-assessment-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e2529-111">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Threat assessment permissions](/graph/permissions-reference#threat-assessment-permissions).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="e2529-112">常见用例</span><span class="sxs-lookup"><span data-stu-id="e2529-112">Common use cases</span></span>

<span data-ttu-id="e2529-113">Microsoft Graph 威胁评估 API 提供了用来列出、创建和获取威胁评估请求以及检索评估结果的方法。</span><span class="sxs-lookup"><span data-stu-id="e2529-113">The Microsoft Graph threat assessment API provides methods to list, create, and get threat assessment requests and retrieve the assessment results.</span></span>

| <span data-ttu-id="e2529-114">用例</span><span class="sxs-lookup"><span data-stu-id="e2529-114">Use cases</span></span> | <span data-ttu-id="e2529-115">REST 资源</span><span class="sxs-lookup"><span data-stu-id="e2529-115">REST resources</span></span> | <span data-ttu-id="e2529-116">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e2529-116">See also</span></span> |
|:----------|:---------------|:---------|
| <span data-ttu-id="e2529-117">列出、创建和获取威胁评估请求</span><span class="sxs-lookup"><span data-stu-id="e2529-117">List, create, and get threat assessment requests</span></span> | [<span data-ttu-id="e2529-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-118">threatAssessmentRequest</span></span>](../resources/threatassessmentrequest.md)<br> [<span data-ttu-id="e2529-119">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-119">mailAssessmentRequest</span></span>](../resources/mailAssessmentRequest.md)<br> [<span data-ttu-id="e2529-120">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-120">emailFileAssessmentRequest</span></span>](../resources/emailFileAssessmentRequest.md)<br> [<span data-ttu-id="e2529-121">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-121">fileAssessmentRequest</span></span>](../resources/fileAssessmentRequest.md)<br> [<span data-ttu-id="e2529-122">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-122">urlAssessmentRequest</span></span>](../resources/urlAssessmentRequest.md)<br> | [<span data-ttu-id="e2529-123">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-123">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md)<br> [<span data-ttu-id="e2529-124">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-124">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md)<br> [<span data-ttu-id="e2529-125">列出 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e2529-125">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) |
| <span data-ttu-id="e2529-126">获取威胁评估结果</span><span class="sxs-lookup"><span data-stu-id="e2529-126">Get threat assessment results</span></span> | [<span data-ttu-id="e2529-127">threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="e2529-127">threatAssessmentResult</span></span>](../resources/threatassessmentresult.md) | [<span data-ttu-id="e2529-128">获取 threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="e2529-128">Get threatAssessmentResult</span></span>](../api/threatassessmentrequest-get.md#example-5-expand-threat-assessment-results-for-a-request)|

## <a name="next-steps"></a><span data-ttu-id="e2529-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e2529-129">Next steps</span></span>

<span data-ttu-id="e2529-130">借助威胁评估资源和 API，可通过新方式使用 Microsoft Graph 与用户交互并管理他们的用户体验。</span><span class="sxs-lookup"><span data-stu-id="e2529-130">Threat assessment resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="e2529-131">要了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="e2529-131">To learn more:</span></span>

- <span data-ttu-id="e2529-132">向下钻取[威胁评估请求](../resources/threatassessmentrequest.md)和[威胁评估结果](../resources/threatAssessmentResult.md)资源的[方法](../resources/threatassessmentrequest.md#methods)、[属性](../resources/threatassessmentrequest.md#properties)和[关系](../resources/threatassessmentrequest.md#relationships)。</span><span class="sxs-lookup"><span data-stu-id="e2529-132">Drill down on the [methods](../resources/threatassessmentrequest.md#methods), [properties](../resources/threatassessmentrequest.md#properties), and [relationships](../resources/threatassessmentrequest.md#relationships) of the [threat assessment request](../resources/threatassessmentrequest.md) and [threat asessment result](../resources/threatAssessmentResult.md) resources.</span></span>
- <span data-ttu-id="e2529-133">请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="e2529-133">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


