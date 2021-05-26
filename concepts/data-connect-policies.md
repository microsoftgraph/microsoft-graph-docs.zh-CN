---
title: Microsoft Graph 数据连接策略和许可
description: 介绍支持的策略以及如何为组织分配 ISV 访问 SKU。
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: b550976f6fde1af5335fb328a9aaef8f48dea33d
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629327"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a><span data-ttu-id="0dcb1-103">Microsoft Graph 数据连接策略和计费</span><span class="sxs-lookup"><span data-stu-id="0dcb1-103">Microsoft Graph Data Connect policies and billing</span></span>

<span data-ttu-id="0dcb1-104">Microsoft Graph 数据连接使用 [Azure 托管应用程序](/azure/managed-applications/overview)，允许你在 Azure 环境中创建和部署解决方案。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-104">Microsoft Graph Data Connect uses [Azure managed applications](/azure/managed-applications/overview) to allow you to create and deploy your solutions in your Azure environment.</span></span> <span data-ttu-id="0dcb1-105">托管应用程序允许你支持某些 Azure 策略，让客户能够更加信心十足并舒适地使用你的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-105">Managed applications allow you to support certain Azure policies, giving customers greater confidence and comfortability when using your applications.</span></span>

## <a name="policies"></a><span data-ttu-id="0dcb1-106">策略</span><span class="sxs-lookup"><span data-stu-id="0dcb1-106">Policies</span></span>

<span data-ttu-id="0dcb1-107">对于使用 Microsoft 365 数据构建的 Azure 托管应用程序，支持使用以下 Azure 策略：</span><span class="sxs-lookup"><span data-stu-id="0dcb1-107">The following Azure policies are supported for an Azure managed application built using Microsoft 365 data:</span></span>

- [<span data-ttu-id="0dcb1-108">Azure 存储和 ADLS Gen 2 必需策略</span><span class="sxs-lookup"><span data-stu-id="0dcb1-108">Azure Storage and ADLS Gen 2 required policy</span></span>](/azure/storage/common/policy-reference)
- [<span data-ttu-id="0dcb1-109">ADLS Gen1 必需策略</span><span class="sxs-lookup"><span data-stu-id="0dcb1-109">ADLS Gen1 required policy</span></span>](/azure/data-lake-store/policy-reference)

> [!NOTE]
> <span data-ttu-id="0dcb1-110">Azure Data Lake Store Gen 1 和 Gen 2 使用不同的策略，因为 ADLS Gen 2 实施 Azure 存储。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-110">Azure Data Lake Store Gen 1 and Gen 2 use different policies because ADLS Gen 2 implements Azure Storage.</span></span>

<span data-ttu-id="0dcb1-111">在 Azure 应用市场发布过程中选择任何策略时，将为应用程序的所有安装检查并实施策略合规性状态。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-111">When you select any of the policies during Azure marketplace publishing, the policy compliance status will be checked and enforced for all installations of your application.</span></span> <span data-ttu-id="0dcb1-112">在数据请求过程中，将向数据审批者显示合规的所有选定策略。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-112">All selected policies that are compliant will be shown to the data approvers as part of the data request.</span></span> <span data-ttu-id="0dcb1-113">任何策略合规性违规行为将导致管道运行失败并停止数据提取。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-113">Any policy compliance violation would cause the pipeline run to fail and stop the data extraction.</span></span>

## <a name="billing-for-microsoft-graph-data-connect"></a><span data-ttu-id="0dcb1-114">Microsoft Graph 数据连接计费</span><span class="sxs-lookup"><span data-stu-id="0dcb1-114">Billing for Microsoft Graph Data Connect</span></span>

<span data-ttu-id="0dcb1-115">账单将与你正在使用的 Azure 数据工厂的 Azure 订阅相关联。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-115">The bill will be associated with the Azure Subscription of the Azure Data Factory you are using.</span></span> <span data-ttu-id="0dcb1-116">此新计费模型的价格基于正在访问的 Microsoft Graph 对象的数量来确定。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-116">The price in this new billing model is based on the number of Microsoft Graph objects you are accessing.</span></span>

<span data-ttu-id="0dcb1-117">虽然此新计费功能仍为预览版本，但价格已确定为每 1,000 个 Microsoft Graph 对象 $0.375。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-117">While this new billing capability is in preview, the rate is $0.375 for 1,000 Microsoft Graph objects.</span></span> <span data-ttu-id="0dcb1-118">例如，如果访问对象总计 10,000 个，你将收到 $3.75 的 Azure 账单。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-118">For example, if you access 10,000 total objects, you will receive an Azure bill for $3.75.</span></span> <span data-ttu-id="0dcb1-119">预览期结束时，费用将改为每 1,000 个 Microsoft Graph 对象 $0.75。</span><span class="sxs-lookup"><span data-stu-id="0dcb1-119">At the end of the preview period, the rate will be $0.75 per 1,000 Microsoft Graph objects.</span></span>

<span data-ttu-id="0dcb1-120">不会收费的目录对象包括：</span><span class="sxs-lookup"><span data-stu-id="0dcb1-120">Directory objects that will not be charged are:</span></span>

- <span data-ttu-id="0dcb1-121">BasicDataSet_v0.User</span><span class="sxs-lookup"><span data-stu-id="0dcb1-121">BasicDataSet_v0.User</span></span>
- <span data-ttu-id="0dcb1-122">BasicDataSet_v0.MailboxSettings</span><span class="sxs-lookup"><span data-stu-id="0dcb1-122">BasicDataSet_v0.MailboxSettings</span></span>
- <span data-ttu-id="0dcb1-123">BasicDataSet_v0.Manager</span><span class="sxs-lookup"><span data-stu-id="0dcb1-123">BasicDataSet_v0.Manager</span></span>
- <span data-ttu-id="0dcb1-124">BasicDataSet_v0.DirectReport</span><span class="sxs-lookup"><span data-stu-id="0dcb1-124">BasicDataSet_v0.DirectReport</span></span>

## <a name="see-also"></a><span data-ttu-id="0dcb1-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0dcb1-125">See also</span></span>

- [<span data-ttu-id="0dcb1-126">Azure 存储策略</span><span class="sxs-lookup"><span data-stu-id="0dcb1-126">Azure Storage policies</span></span>](/azure/storage/common/policy-reference)
- [<span data-ttu-id="0dcb1-127">Microsoft Graph 数据连接计费</span><span class="sxs-lookup"><span data-stu-id="0dcb1-127">Microsoft Graph Data Connect billing</span></span>](https://azure.microsoft.com/pricing/details/graph-data-connect/)
- [<span data-ttu-id="0dcb1-128">Azure 托管应用程序</span><span class="sxs-lookup"><span data-stu-id="0dcb1-128">Azure managed applications</span></span>](/azure/managed-applications/overview)
- [<span data-ttu-id="0dcb1-129">用户选择和筛选</span><span class="sxs-lookup"><span data-stu-id="0dcb1-129">User selection and filtering</span></span>](data-connect-filtering.md)
- [<span data-ttu-id="0dcb1-130">数据连接常见问题解答</span><span class="sxs-lookup"><span data-stu-id="0dcb1-130">Data Connect frequently asked questions</span></span>](data-connect-faq.md)
