---
title: 使用 Microsoft Graph 中个人资料 API 自定义个人资料卡（预览版）
description: 本文介绍如何通过使其他属性可见或添加自定义属性来自定义个人资料卡。
author: PollyNincevic
localization\_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 749851d32678617ab2c7b7b7d16d063686f815ce
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352345"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a><span data-ttu-id="fe83c-103">使用 Microsoft Graph 中的个人资料卡 API 向个人资料卡添加其他属性（预览版）</span><span class="sxs-lookup"><span data-stu-id="fe83c-103">Add additional properties to the profile card using the profile card API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="fe83c-104">在 Microsoft 365 的 [个人资料卡](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501)上，可以找到由组织存储和维护的有关用户的信息，例如 **职位名称** 或 **办公室位置**。</span><span class="sxs-lookup"><span data-stu-id="fe83c-104">On the [profile card](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) in Microsoft 365, you can find information about users that is stored and maintained by your organization, for example **Job title** or **Office location**.</span></span>

<span data-ttu-id="fe83c-105">使用 [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) 资源通过以下方式在组织的个人资料卡上显示Azure AD 的其他属性：</span><span class="sxs-lookup"><span data-stu-id="fe83c-105">Use the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource to show additional properties from Azure AD on profile cards for an organization, by:</span></span>

* <span data-ttu-id="fe83c-106">使其他属性可见</span><span class="sxs-lookup"><span data-stu-id="fe83c-106">Making additional attributes visible</span></span>
* <span data-ttu-id="fe83c-107">添加自定义属性</span><span class="sxs-lookup"><span data-stu-id="fe83c-107">Adding custom attributes</span></span>

<span data-ttu-id="fe83c-108">其他属性将显示在 Microsoft 365 中的个人资料卡的 **联系人** 部分中。</span><span class="sxs-lookup"><span data-stu-id="fe83c-108">Additional properties will display in the **Contact** section of the profile card in Microsoft 365.</span></span>

> [!NOTE]
> <span data-ttu-id="fe83c-109">使用委派权限的 **profileCardProperty** 资源上的操作要求已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="fe83c-109">Operations on the **profileCardProperty** resource that use delegated permissions require the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="make-additional-attributes-visible"></a><span data-ttu-id="fe83c-110">使其他属性可见</span><span class="sxs-lookup"><span data-stu-id="fe83c-110">Make additional attributes visible</span></span>

<span data-ttu-id="fe83c-111">可以在用户的​​个人资料卡上显示 Azure Active Directory（Azure AD）的以下属性。</span><span class="sxs-lookup"><span data-stu-id="fe83c-111">You can make the following attributes from Azure Active Directory (Azure AD) visible on users' profile cards.</span></span> <span data-ttu-id="fe83c-112">这些属性 *不区分大小写*：</span><span class="sxs-lookup"><span data-stu-id="fe83c-112">These attributes are *not case-sensitive*:</span></span>

* `UserPrincipalName`
* `Fax`
* `StreetAddress`
* `PostalCode`
* `StateOrProvince`
* `Alias`

<span data-ttu-id="fe83c-113">下表显示了Azure AD 属性如何与 Microsoft Graph [user](/graph/api/resources/user?view=graph-rest-beta) 实体的属性相对应。</span><span class="sxs-lookup"><span data-stu-id="fe83c-113">The following table shows how the Azure AD attributes correspond with properties of the Microsoft Graph [user](/graph/api/resources/user?view=graph-rest-beta) entity.</span></span>

| <span data-ttu-id="fe83c-114">Azure AD 属性</span><span class="sxs-lookup"><span data-stu-id="fe83c-114">Azure AD attribute</span></span> | <span data-ttu-id="fe83c-115">用户实体属性</span><span class="sxs-lookup"><span data-stu-id="fe83c-115">User entity property</span></span> |
| ------------------ | -------------------- |
| <span data-ttu-id="fe83c-116">UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe83c-116">UserPrincipalName</span></span> | <span data-ttu-id="fe83c-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe83c-117">userPrincipalName</span></span> |
| <span data-ttu-id="fe83c-118">Fax</span><span class="sxs-lookup"><span data-stu-id="fe83c-118">Fax</span></span> | <span data-ttu-id="fe83c-119">faxNumber</span><span class="sxs-lookup"><span data-stu-id="fe83c-119">faxNumber</span></span> |
| <span data-ttu-id="fe83c-120">StreetAddress</span><span class="sxs-lookup"><span data-stu-id="fe83c-120">StreetAddress</span></span> | <span data-ttu-id="fe83c-121">streetAddress</span><span class="sxs-lookup"><span data-stu-id="fe83c-121">streetAddress</span></span> |
| <span data-ttu-id="fe83c-122">PostalCode</span><span class="sxs-lookup"><span data-stu-id="fe83c-122">PostalCode</span></span> | <span data-ttu-id="fe83c-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="fe83c-123">postalCode</span></span> |
| <span data-ttu-id="fe83c-124">StateOrProvince</span><span class="sxs-lookup"><span data-stu-id="fe83c-124">StateOrProvince</span></span> | <span data-ttu-id="fe83c-125">state</span><span class="sxs-lookup"><span data-stu-id="fe83c-125">state</span></span> |
| <span data-ttu-id="fe83c-126">Alias</span><span class="sxs-lookup"><span data-stu-id="fe83c-126">Alias</span></span> | <span data-ttu-id="fe83c-127">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fe83c-127">mailNickname</span></span> |

<span data-ttu-id="fe83c-128">您可以通过配置您的 [组织设置](/graph/api/resources/organizationsettings?view=graph-rest-beta)并在 Microsoft Graph 中将属性添加为 **profileCardProperty** 的 **directoryPropertyName** 属性，将这些属性中的任何属性添加到配置文件卡片中。</span><span class="sxs-lookup"><span data-stu-id="fe83c-128">You can add any of these attributes to the profile card by configuring your [organization settings](/graph/api/resources/organizationsettings?view=graph-rest-beta) and adding the attribute as the **directoryPropertyName** property of a **profileCardProperty** in Microsoft Graph.</span></span> <span data-ttu-id="fe83c-129">当使其他属性可见时，必须使用 `en-us` 的属性名称。</span><span class="sxs-lookup"><span data-stu-id="fe83c-129">When you make additional attributes visible, you must use the property names for `en-us`.</span></span> <span data-ttu-id="fe83c-130">不必添加本地化值。</span><span class="sxs-lookup"><span data-stu-id="fe83c-130">You don't have to add localized values.</span></span> <span data-ttu-id="fe83c-131">其他属性将自动以用户为 Microsoft 365 指定的语言设置显示。</span><span class="sxs-lookup"><span data-stu-id="fe83c-131">The additional properties will automatically be shown in the language settings that the user has specified for Microsoft 365.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fe83c-132">向个人资料卡添加属性时，最多需要 24 小时才能显示添加内容。</span><span class="sxs-lookup"><span data-stu-id="fe83c-132">When adding an attribute to profile card, it takes up to 24 hours for the addition to be displayed.</span></span>

## <a name="example"></a><span data-ttu-id="fe83c-133">示例</span><span class="sxs-lookup"><span data-stu-id="fe83c-133">Example</span></span>

<span data-ttu-id="fe83c-134">下面的示例显示 `Alias` 配置文件卡片上的属性。</span><span class="sxs-lookup"><span data-stu-id="fe83c-134">The following example displays the `Alias` attribute on the profile card.</span></span>

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

<span data-ttu-id="fe83c-135">如果成功，则响应在响应正文中返回 `201 OK` 响应代码和 **profileCardProperty** 对象。</span><span class="sxs-lookup"><span data-stu-id="fe83c-135">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="fe83c-136">属性的值 `Alias` 将显示在用户的配置文件卡片上。</span><span class="sxs-lookup"><span data-stu-id="fe83c-136">The value for the `Alias` attribute would be displayed on a user's profile card.</span></span>

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a><span data-ttu-id="fe83c-137">添加自定义属性</span><span class="sxs-lookup"><span data-stu-id="fe83c-137">Adding custom attributes</span></span>

<span data-ttu-id="fe83c-138">可以通过配置组织设置并在 Microsoft Graph 中[将相应的值添加为profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta)，将 15 个 Azure AD [自定义扩展属性](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)中的任何一个添加到用户的个人资料卡中。</span><span class="sxs-lookup"><span data-stu-id="fe83c-138">You can add any of the 15 Azure AD [custom extension attributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) to users' profile cards by configuring your organization settings and [adding the corresponding value as a profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) in Microsoft Graph.</span></span> <span data-ttu-id="fe83c-139">一次可以添加一个 **profileCardProperty** 资源。</span><span class="sxs-lookup"><span data-stu-id="fe83c-139">You can add one **profileCardProperty** resource at a time.</span></span>

<span data-ttu-id="fe83c-140">所做的更改最多需要 24 小时才能显示在个人资料卡上。</span><span class="sxs-lookup"><span data-stu-id="fe83c-140">It takes up to 24 hours for the changes to show on profile cards.</span></span>

<span data-ttu-id="fe83c-141">自定义属性不可搜索，不能用于在 Microsoft 应用程序和服务中搜索人员。</span><span class="sxs-lookup"><span data-stu-id="fe83c-141">Custom properties are not searchable and can't be used to search for people across Microsoft apps and services.</span></span>

<span data-ttu-id="fe83c-142">下表显示了 Azure AD 自定义扩展属性名称如何与 [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) 资源的 **directoryPropertyName** 属性支持值相对应。</span><span class="sxs-lookup"><span data-stu-id="fe83c-142">The following table shows how the Azure AD custom extension attribute names correspond to the supported values for the **directoryPropertyName** property of the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource.</span></span> <span data-ttu-id="fe83c-143">这些 Azure AD 自定义扩展属性名称 *不区分大小写*：</span><span class="sxs-lookup"><span data-stu-id="fe83c-143">These Azure AD custom extension attribute names are *not case-sensitive*:</span></span>

| <span data-ttu-id="fe83c-144">Azure AD 自定义扩展属性</span><span class="sxs-lookup"><span data-stu-id="fe83c-144">Azure AD custom extension attribute</span></span> | <span data-ttu-id="fe83c-145">指定为 directoryPropertyName 的值</span><span class="sxs-lookup"><span data-stu-id="fe83c-145">Value to specify as directoryPropertyName</span></span> |
| ----------------------------------- | ----------------------------------------- |
| <span data-ttu-id="fe83c-146">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="fe83c-146">extensionAttribute1</span></span> | <span data-ttu-id="fe83c-147">customAttribute1</span><span class="sxs-lookup"><span data-stu-id="fe83c-147">customAttribute1</span></span> |
| <span data-ttu-id="fe83c-148">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="fe83c-148">extensionAttribute2</span></span> | <span data-ttu-id="fe83c-149">customAttribute2</span><span class="sxs-lookup"><span data-stu-id="fe83c-149">customAttribute2</span></span> |
| <span data-ttu-id="fe83c-150">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="fe83c-150">extensionAttribute3</span></span> | <span data-ttu-id="fe83c-151">customAttribute3</span><span class="sxs-lookup"><span data-stu-id="fe83c-151">customAttribute3</span></span> |
| <span data-ttu-id="fe83c-152">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="fe83c-152">extensionAttribute4</span></span> | <span data-ttu-id="fe83c-153">customAttribute4</span><span class="sxs-lookup"><span data-stu-id="fe83c-153">customAttribute4</span></span> |
| <span data-ttu-id="fe83c-154">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="fe83c-154">extensionAttribute5</span></span> | <span data-ttu-id="fe83c-155">customAttribute5</span><span class="sxs-lookup"><span data-stu-id="fe83c-155">customAttribute5</span></span> |
| <span data-ttu-id="fe83c-156">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="fe83c-156">extensionAttribute6</span></span> | <span data-ttu-id="fe83c-157">customAttribute6</span><span class="sxs-lookup"><span data-stu-id="fe83c-157">customAttribute6</span></span> |
| <span data-ttu-id="fe83c-158">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="fe83c-158">extensionAttribute7</span></span> | <span data-ttu-id="fe83c-159">customAttribute7</span><span class="sxs-lookup"><span data-stu-id="fe83c-159">customAttribute7</span></span> |
| <span data-ttu-id="fe83c-160">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="fe83c-160">extensionAttribute8</span></span> | <span data-ttu-id="fe83c-161">customAttribute8</span><span class="sxs-lookup"><span data-stu-id="fe83c-161">customAttribute8</span></span> |
| <span data-ttu-id="fe83c-162">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="fe83c-162">extensionAttribute9</span></span> | <span data-ttu-id="fe83c-163">customAttribute9</span><span class="sxs-lookup"><span data-stu-id="fe83c-163">customAttribute9</span></span> |
| <span data-ttu-id="fe83c-164">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="fe83c-164">extensionAttribute10</span></span> | <span data-ttu-id="fe83c-165">customAttribute10</span><span class="sxs-lookup"><span data-stu-id="fe83c-165">customAttribute10</span></span> |
| <span data-ttu-id="fe83c-166">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="fe83c-166">extensionAttribute11</span></span> | <span data-ttu-id="fe83c-167">customAttribute11</span><span class="sxs-lookup"><span data-stu-id="fe83c-167">customAttribute11</span></span> |
| <span data-ttu-id="fe83c-168">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="fe83c-168">extensionAttribute12</span></span> | <span data-ttu-id="fe83c-169">customAttribute12</span><span class="sxs-lookup"><span data-stu-id="fe83c-169">customAttribute12</span></span> |
| <span data-ttu-id="fe83c-170">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="fe83c-170">extensionAttribute13</span></span> | <span data-ttu-id="fe83c-171">customAttribute13</span><span class="sxs-lookup"><span data-stu-id="fe83c-171">customAttribute13</span></span> |
| <span data-ttu-id="fe83c-172">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="fe83c-172">extensionAttribute14</span></span> | <span data-ttu-id="fe83c-173">customAttribute14</span><span class="sxs-lookup"><span data-stu-id="fe83c-173">customAttribute14</span></span> |
| <span data-ttu-id="fe83c-174">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="fe83c-174">extensionAttribute15</span></span> | <span data-ttu-id="fe83c-175">customAttribute15</span><span class="sxs-lookup"><span data-stu-id="fe83c-175">customAttribute15</span></span> |

## <a name="example"></a><span data-ttu-id="fe83c-176">示例</span><span class="sxs-lookup"><span data-stu-id="fe83c-176">Example</span></span>

<span data-ttu-id="fe83c-177">下面的示例使用显示名称 **成本中心** 将第一个 Azure AD 自定义扩展属性添加到个人资料卡。</span><span class="sxs-lookup"><span data-stu-id="fe83c-177">The following example adds the first Azure AD custom extension attribute to the profile card, using the display name **Cost center**.</span></span> <span data-ttu-id="fe83c-178">对于将语言设置设置为德语的用户，显示名称将为 **Kostenstelle**。</span><span class="sxs-lookup"><span data-stu-id="fe83c-178">For users that have set their language settings to German, the display name will be **Kostenstelle**.</span></span>

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

<span data-ttu-id="fe83c-179">如果语言不受支持，则将使用默认值显示属性名称。</span><span class="sxs-lookup"><span data-stu-id="fe83c-179">If a language is not supported, the property name will be shown with the default value.</span></span>

<span data-ttu-id="fe83c-180">如果成功，则响应在响应正文中返回 `201 OK` 响应代码和 **profileCardProperty** 对象。</span><span class="sxs-lookup"><span data-stu-id="fe83c-180">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="fe83c-181">在此示例中，你可以假设对于已在个人资料卡上将其语言设置为德语的所有用户，个人资料卡显示 **Kostenstelle**。</span><span class="sxs-lookup"><span data-stu-id="fe83c-181">In this example you can assume that the profile card displays **Kostenstelle** for all users that have set their language settings to German on the profile card.</span></span> <span data-ttu-id="fe83c-182">对于所有其他用户，**成本中心** 将显示在个人资料卡上。</span><span class="sxs-lookup"><span data-stu-id="fe83c-182">For all other users, **Cost center** will be displayed on the profile card.</span></span>

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="fe83c-183">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fe83c-183">See also</span></span>

- [<span data-ttu-id="fe83c-184">查找 Microsoft 365 租户 ID</span><span class="sxs-lookup"><span data-stu-id="fe83c-184">Find your Microsoft 365 tenant ID</span></span>](/onedrive/find-your-office-365-tenant-id)
- [<span data-ttu-id="fe83c-185">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe83c-185">onPremisesExtensionAttributes resource type</span></span>](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)
- [<span data-ttu-id="fe83c-186">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="fe83c-186">User resource type</span></span>](/graph/api/resources/user?view=graph-rest-beta)
- [<span data-ttu-id="fe83c-187">Graph 浏览器</span><span class="sxs-lookup"><span data-stu-id="fe83c-187">Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)
- [<span data-ttu-id="fe83c-188">Get profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="fe83c-188">Get profileCardProperty</span></span>](/graph/api/profilecardproperty-get?view=graph-rest-beta)
