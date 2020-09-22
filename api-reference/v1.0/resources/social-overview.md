---
title: 使用 Microsoft Graph API 在应用程序中集成人员智能
description: Microsoft Graph 允许访问相关人员的有用数据以及与之交互的文档。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 154762d1658503a25ffe2ec39bdf602f4a9d2b8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970542"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-intelligence-in-an-app"></a><span data-ttu-id="eda7c-103">使用 Microsoft Graph API 在应用程序中集成人员智能</span><span class="sxs-lookup"><span data-stu-id="eda7c-103">Use the Microsoft Graph API to integrate people intelligence in an app</span></span>

<span data-ttu-id="eda7c-104">Microsoft Graph 允许访问相关人员的有用数据以及与之交互的文档。</span><span class="sxs-lookup"><span data-stu-id="eda7c-104">Microsoft Graph enables access to useful data about people and documents they interact with.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="eda7c-105">聚合并提取有关人员的特定信息</span><span class="sxs-lookup"><span data-stu-id="eda7c-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="eda7c-106">功能：人员</span><span class="sxs-lookup"><span data-stu-id="eda7c-106">Feature: People</span></span>

<span data-ttu-id="eda7c-107">可使用 [person](../resources/person.md) 资源和人员 API 从邮件、联系人和社交网络中收集某位用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="eda7c-107">You can use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="eda7c-108">根据多个通信和协作模式及业务关系按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="eda7c-108">The results are ordered by their relevance based on multiple communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="eda7c-109">通过此 API 可基于自己的条件对人员进行浏览、排序、选择、筛选或搜索。</span><span class="sxs-lookup"><span data-stu-id="eda7c-109">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

<span data-ttu-id="eda7c-110">有关应用场景及示例，请参阅[获取相关人员的信息](/graph/people-example)。</span><span class="sxs-lookup"><span data-stu-id="eda7c-110">For scenarios and examples, see [Get information about relevant people](/graph/people-example).</span></span>

<span data-ttu-id="eda7c-111">若要使用此 API，请参阅下列内容：</span><span class="sxs-lookup"><span data-stu-id="eda7c-111">To use the API, see the following:</span></span>

- [<span data-ttu-id="eda7c-112">列出人员</span><span class="sxs-lookup"><span data-stu-id="eda7c-112">List people</span></span>](../api/user-list-people.md)


## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="eda7c-113">帮助用户获得最相关的工作文档</span><span class="sxs-lookup"><span data-stu-id="eda7c-113">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="eda7c-114">功能：文档见解</span><span class="sxs-lookup"><span data-stu-id="eda7c-114">Feature: Document insights</span></span>

<span data-ttu-id="eda7c-115">使用见解 API 为用户标识最相关的文档：</span><span class="sxs-lookup"><span data-stu-id="eda7c-115">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="eda7c-116">列出用户[常用的](../api/insights-list-trending.md)文档</span><span class="sxs-lookup"><span data-stu-id="eda7c-116">List documents [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="eda7c-117">列出用户[使用的](../api/insights-list-used.md)文档</span><span class="sxs-lookup"><span data-stu-id="eda7c-117">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="eda7c-118">列出[与用户共享或由用户共享的](../api/insights-list-shared.md)文档</span><span class="sxs-lookup"><span data-stu-id="eda7c-118">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="whats-new"></a><span data-ttu-id="eda7c-119">最近更新</span><span class="sxs-lookup"><span data-stu-id="eda7c-119">What's new</span></span>
<span data-ttu-id="eda7c-120">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="eda7c-120">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
