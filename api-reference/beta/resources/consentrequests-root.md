---
title: Azure Active Directory同意请求
description: 使用 Azure AD 同意请求来管理尝试访问需要管理员同意的应用的用户的请求工作流。
localization_priority: Normal
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: cd4ce281ac79f9f8409685c321255828e50e5122
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971403"
---
# <a name="azure-active-directory-consent-requests"></a><span data-ttu-id="6b6d1-103">Azure Active Directory同意请求</span><span class="sxs-lookup"><span data-stu-id="6b6d1-103">Azure Active Directory consent requests</span></span>

<span data-ttu-id="6b6d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b6d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b6d1-105">Azure Active Directory (Azure AD) 请求可帮助你管理尝试访问需要管理员批准的应用的用户的请求工作流。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-105">Azure Active Directory (Azure AD) consent requests help you manage the request workflow for users attempting to access apps that require admin approval.</span></span>

<span data-ttu-id="6b6d1-106">若要允许用户请求其未经授权应用程序的访问权限或管理员同意以向自己授予同意，请首先启用同意请求工作流。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-106">To allow users to request access or admin consent for applications they're unauthorized to grant consent to themselves, first enable the consent request workflow.</span></span> 

>[!NOTE]
><span data-ttu-id="6b6d1-107">当前 API 仅限于配置工作流和读取请求列表。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-107">The current APIs are limited to configuring the workflow and reading the list of requests.</span></span> <span data-ttu-id="6b6d1-108">目前，没有任何方法可用于以编程方式批准或拒绝请求。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-108">At this time, there aren’t any methods available to programmatically approve or deny a request.</span></span> <span data-ttu-id="6b6d1-109">但是，请求的内容可用于重新创建可用于授予管理员同意和批准请求的 URL。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-109">However, the contents of the request can be used to recreate a URL which can be used to grant admin consent and approve a request.</span></span>

<span data-ttu-id="6b6d1-110">同意请求资源类型包括：</span><span class="sxs-lookup"><span data-stu-id="6b6d1-110">The consent request resource types include:</span></span>

* <span data-ttu-id="6b6d1-111">[adminConsentRequestPolicy：](../resources/adminconsentrequestpolicy.md)指定可在整个租户中创建和管理应用同意请求的策略。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-111">[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md): Specifies the policy by which app consent requests can be created and managed for the entire tenant.</span></span> <span data-ttu-id="6b6d1-112">每个租户只有一个 **adminConsentRequestPolicy。**</span><span class="sxs-lookup"><span data-stu-id="6b6d1-112">There is a single **adminConsentRequestPolicy** per tenant.</span></span>
* <span data-ttu-id="6b6d1-113">[appConsentRequest：](../resources/appconsentrequest.md)表示特定应用程序的 **userConsentRequests** 集合的请求。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-113">[appConsentRequest](../resources/appconsentrequest.md): A request that represents a collection of **userConsentRequests** for a specific application.</span></span>
* <span data-ttu-id="6b6d1-114">[userConsentRequest：](../resources/userconsentrequest.md)用户创建以使用需要管理员同意才能访问的应用的请求。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-114">[userConsentRequest](../resources/userconsentrequest.md): A request created by a user to use an app that requires admin consent to access.</span></span>
* <span data-ttu-id="6b6d1-115">[appConsentRequestScope：](../resources/appconsentrequestscope.md)包含为应用程序请求的动态权限范围的详细信息的资源。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-115">[appConsentRequestScope](../resources/appconsentrequestscope.md): A resource that contains details of the dynamic permission scopes being requested for an application.</span></span>  

## <a name="methods"></a><span data-ttu-id="6b6d1-116">方法</span><span class="sxs-lookup"><span data-stu-id="6b6d1-116">Methods</span></span>

<span data-ttu-id="6b6d1-117">下表列出了可用于与同意请求资源进行交互的方法。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-117">The following table lists the methods that you can use to interact with consent request resources.</span></span>

| <span data-ttu-id="6b6d1-118">方法</span><span class="sxs-lookup"><span data-stu-id="6b6d1-118">Method</span></span>           | <span data-ttu-id="6b6d1-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="6b6d1-119">Return type</span></span>    |<span data-ttu-id="6b6d1-120">说明</span><span class="sxs-lookup"><span data-stu-id="6b6d1-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b6d1-121">获取 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="6b6d1-121">Get adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-get.md) | <span data-ttu-id="6b6d1-122">[adminConsentRequestPolicy](adminconsentrequestpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-122">[adminConsentRequestPolicy](adminconsentrequestpolicy.md) collection</span></span> | <span data-ttu-id="6b6d1-123">读取 [adminConsentRequestPolicy 的属性](adminconsentrequestpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-123">Read the properties of the [adminConsentRequestPolicy](adminconsentrequestpolicy.md).</span></span> |
|[<span data-ttu-id="6b6d1-124">更新 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="6b6d1-124">Update adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-update.md) | <span data-ttu-id="6b6d1-125">[adminConsentRequestPolicy](adminconsentrequestpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-125">[adminConsentRequestPolicy](adminconsentrequestpolicy.md) collection</span></span> | <span data-ttu-id="6b6d1-126">设置 [adminConsentRequestPolicy 的配置](adminconsentrequestpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-126">Set configurations for the [adminConsentRequestPolicy](adminconsentrequestpolicy.md).</span></span> |
|[<span data-ttu-id="6b6d1-127">列出 appConsentRequests </span><span class="sxs-lookup"><span data-stu-id="6b6d1-127">List appConsentRequests </span></span>](../api/appconsentrequest-list.md) | <span data-ttu-id="6b6d1-128">[appConsentRequest](appconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-128">[appConsentRequest](appconsentrequest.md) collection</span></span> | <span data-ttu-id="6b6d1-129">检索 [appConsentRequest](appconsentrequest.md) 对象及其属性的集合。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-129">Retrieve a collection of [appConsentRequest](appconsentrequest.md) objects and their properties.</span></span> |
|[<span data-ttu-id="6b6d1-130">获取 appConsentRequest </span><span class="sxs-lookup"><span data-stu-id="6b6d1-130">Get appConsentRequest </span></span>](../api/appconsentrequest-get.md) | <span data-ttu-id="6b6d1-131">[appConsentRequest](appconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-131">[appConsentRequest](appconsentrequest.md) collection</span></span> | <span data-ttu-id="6b6d1-132">读取 [appConsentRequest](appconsentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-132">Read an [appConsentRequest](appconsentrequest.md) object.</span></span> |
|[<span data-ttu-id="6b6d1-133">appConsentRequests：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="6b6d1-133">appConsentRequests: filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md) | <span data-ttu-id="6b6d1-134">[appConsentRequest](../resources/appconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-134">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span> | <span data-ttu-id="6b6d1-135">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性，当前用户是这些对象的审阅者，并且用户同意请求的状态为 `InProgress` 。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-135">Read the properties of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the user consent request is `InProgress`.</span></span> |
|[<span data-ttu-id="6b6d1-136">获取 userConsentRequest </span><span class="sxs-lookup"><span data-stu-id="6b6d1-136">Get userConsentRequest </span></span>](../api/userconsentrequest-get.md) | <span data-ttu-id="6b6d1-137">[userConsentRequest](userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-137">[userConsentRequest](userconsentrequest.md) collection</span></span> | <span data-ttu-id="6b6d1-138">读取 [appConsentRequest](userconsentrequest.md) 的 [userConsentRequest 对象](appconsentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-138">Read a [userConsentRequest](userconsentrequest.md) object for an [appConsentRequest](appconsentrequest.md).</span></span> |
|[<span data-ttu-id="6b6d1-139">列出 userConsentRequests </span><span class="sxs-lookup"><span data-stu-id="6b6d1-139">List userConsentRequests </span></span>](../api/userconsentrequest-list.md) | <span data-ttu-id="6b6d1-140">[userConsentRequest](userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-140">[userConsentRequest](userconsentrequest.md) collection</span></span> | <span data-ttu-id="6b6d1-141">检索 [appConsentRequest 的 userConsentRequest](userconsentrequest.md) [对象的集合](appconsentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-141">Retrieve a collection of [userConsentRequest](userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md).</span></span> |
|[<span data-ttu-id="6b6d1-142">userConsentRequest：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="6b6d1-142">userConsentRequest: filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md) | <span data-ttu-id="6b6d1-143">[appConsentRequests](../resources/userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6d1-143">[appConsentRequests](../resources/userconsentrequest.md) collection</span></span> | <span data-ttu-id="6b6d1-144">读取当前用户是审阅者的[appConsentRequest 的](appconsentrequest.md) [userConsentRequest](../resources/userconsentrequest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-144">Read the properties of [userConsentRequest](../resources/userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md) for which the current user is the reviewer.</span></span> |

## <a name="role-and-delegated-permission-authorization-checks"></a><span data-ttu-id="6b6d1-145">角色和委派权限授权检查</span><span class="sxs-lookup"><span data-stu-id="6b6d1-145">Role and delegated permission authorization checks</span></span>

<span data-ttu-id="6b6d1-146">以下目录角色是呼叫用户管理请求工作流或读取请求列表所需的。</span><span class="sxs-lookup"><span data-stu-id="6b6d1-146">The following directory roles are required for a calling user to manage the requests workflow or read the list of requests.</span></span>

| <span data-ttu-id="6b6d1-147">操作</span><span class="sxs-lookup"><span data-stu-id="6b6d1-147">Operation</span></span> | <span data-ttu-id="6b6d1-148">委派权限</span><span class="sxs-lookup"><span data-stu-id="6b6d1-148">Delegated permissions</span></span> | <span data-ttu-id="6b6d1-149">呼叫用户的必需目录角色</span><span class="sxs-lookup"><span data-stu-id="6b6d1-149">Required directory role of the calling user</span></span> |
|:------------------|:------------|:--------------------------------------------|
| <span data-ttu-id="6b6d1-150">读取</span><span class="sxs-lookup"><span data-stu-id="6b6d1-150">Read</span></span> | <span data-ttu-id="6b6d1-151">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b6d1-151">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span> | <span data-ttu-id="6b6d1-152">全局管理员、全局读者、云应用管理员和应用程序管理员</span><span class="sxs-lookup"><span data-stu-id="6b6d1-152">Global Administrator, Global Reader, Cloud App Administrator, and Application Administrator</span></span> |

## <a name="see-also"></a><span data-ttu-id="6b6d1-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6b6d1-153">See also</span></span>

- [<span data-ttu-id="6b6d1-154">配置管理员同意工作流 (预览) </span><span class="sxs-lookup"><span data-stu-id="6b6d1-154">Configure the admin consent workflow (preview)</span></span>](/azure/active-directory/manage-apps/configure-admin-consent-workflow?preserve-view=true)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
