---
title: 使用 Microsoft Graph 中的配置文件 API 自定义配置文件卡片（预览）
description: 本文介绍如何通过显示其他属性来自定义配置文件卡片，或添加自定义属性。
author: PollyNincevic
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: dc0c78ecfdf00488c7c9c12969eea8b405be496c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050973"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-api-in-microsoft-graph-preview"></a><span data-ttu-id="f4629-103">使用 Microsoft Graph 中的配置文件 API 将其他属性添加到配置文件卡片（预览）</span><span class="sxs-lookup"><span data-stu-id="f4629-103">Add additional properties to the profile card using the profile API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="f4629-104">在 Microsoft 365 中的[配置文件卡片](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501)中，可以找到组织存储和维护的用户的相关信息，例如**职务**或**办公室位置**。</span><span class="sxs-lookup"><span data-stu-id="f4629-104">On the [profile card](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) in Microsoft 365, you can find information about users that is stored and maintained by your organization, for example **Job title** or **Office location**.</span></span>

<span data-ttu-id="f4629-105">使用[profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta)资源显示来自组织的配置文件卡上的 Azure AD 的其他属性，方法如下：</span><span class="sxs-lookup"><span data-stu-id="f4629-105">Use the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource to show additional properties from Azure AD on profile cards for an organization, by:</span></span>

- <span data-ttu-id="f4629-106">让其他属性可见</span><span class="sxs-lookup"><span data-stu-id="f4629-106">Making additional attributes visible</span></span>

- <span data-ttu-id="f4629-107">添加自定义属性</span><span class="sxs-lookup"><span data-stu-id="f4629-107">Adding custom attributes</span></span>

<span data-ttu-id="f4629-108">其他属性将显示在 Microsoft 365 的配置文件卡片的 "**联系人**" 部分中。</span><span class="sxs-lookup"><span data-stu-id="f4629-108">Additional properties will display in the **Contact** section of the profile card in Microsoft 365.</span></span>

> [!NOTE]
><span data-ttu-id="f4629-109">使用委派权限的**profileCardProperty**资源上的操作要求已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="f4629-109">Operations on the **profileCardProperty** resource that use delegated permissions requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="make-additional-attributes-visible"></a><span data-ttu-id="f4629-110">使其他属性可见</span><span class="sxs-lookup"><span data-stu-id="f4629-110">Make additional attributes visible</span></span>

<span data-ttu-id="f4629-111">你可以在用户配置文件卡上看到 Azure Active Directory （Azure AD）中的以下属性。</span><span class="sxs-lookup"><span data-stu-id="f4629-111">You can make the following attributes from Azure Active Directory (Azure AD) visible on users' profile cards.</span></span> <span data-ttu-id="f4629-112">这些属性*不区分大小写*：</span><span class="sxs-lookup"><span data-stu-id="f4629-112">These attributes are *not case-sensitive*:</span></span>

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

<span data-ttu-id="f4629-113">下表显示了 Azure AD 属性如何与 Microsoft Graph[用户](/graph/api/resources/user?view=graph-rest-beta)实体的属性相对应。</span><span class="sxs-lookup"><span data-stu-id="f4629-113">The following table shows how the Azure AD attributes correspond with properties of the Microsoft Graph [user](/graph/api/resources/user?view=graph-rest-beta) entity.</span></span>

|<span data-ttu-id="f4629-114">Azure AD 属性</span><span class="sxs-lookup"><span data-stu-id="f4629-114">Azure AD attribute</span></span> |<span data-ttu-id="f4629-115">User entity 属性</span><span class="sxs-lookup"><span data-stu-id="f4629-115">User entity property</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f4629-116">UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4629-116">UserPrincipalName</span></span>|<span data-ttu-id="f4629-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4629-117">userPrincipalName</span></span> |
|<span data-ttu-id="f4629-118">传真</span><span class="sxs-lookup"><span data-stu-id="f4629-118">Fax</span></span>|<span data-ttu-id="f4629-119">faxNumber</span><span class="sxs-lookup"><span data-stu-id="f4629-119">faxNumber</span></span>|
|<span data-ttu-id="f4629-120">StreetAddress</span><span class="sxs-lookup"><span data-stu-id="f4629-120">StreetAddress</span></span>|<span data-ttu-id="f4629-121">streetAddress</span><span class="sxs-lookup"><span data-stu-id="f4629-121">streetAddress</span></span>|
|<span data-ttu-id="f4629-122">PostalCode</span><span class="sxs-lookup"><span data-stu-id="f4629-122">PostalCode</span></span>|<span data-ttu-id="f4629-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="f4629-123">postalCode</span></span>|
|<span data-ttu-id="f4629-124">StateOrProvince</span><span class="sxs-lookup"><span data-stu-id="f4629-124">StateOrProvince</span></span>|<span data-ttu-id="f4629-125">状态</span><span class="sxs-lookup"><span data-stu-id="f4629-125">state</span></span>
|<span data-ttu-id="f4629-126">Alias</span><span class="sxs-lookup"><span data-stu-id="f4629-126">Alias</span></span>|<span data-ttu-id="f4629-127">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f4629-127">mailNickname</span></span>

<span data-ttu-id="f4629-128">您可以通过配置您的[组织设置](/graph/api/resources/organizationsettings?view=graph-rest-beta)并将属性添加为 Microsoft Graph 中**profileCardProperty**的*directoryPropertyName*\* 属性，将这些属性中的任何属性添加到配置文件卡片中。</span><span class="sxs-lookup"><span data-stu-id="f4629-128">You can add any of these attributes to the profile card by configuring your [organization settings](/graph/api/resources/organizationsettings?view=graph-rest-beta) and adding the attribute as the *directoryPropertyName*\* property of a **profileCardProperty** in Microsoft Graph.</span></span> <span data-ttu-id="f4629-129">当您使其他属性可见时，您必须使用的属性名称 `en-us` 。</span><span class="sxs-lookup"><span data-stu-id="f4629-129">When you make additional attributes visible, you must use the property names for `en-us`.</span></span> <span data-ttu-id="f4629-130">您不必添加本地化的值。</span><span class="sxs-lookup"><span data-stu-id="f4629-130">You don't have to add localized values.</span></span> <span data-ttu-id="f4629-131">其他属性将自动显示在用户为 Microsoft 365 指定的语言设置中。</span><span class="sxs-lookup"><span data-stu-id="f4629-131">The additional properties will automatically be shown in the language settings that the user has specified for Microsoft 365.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f4629-132">将属性添加到配置文件卡片时，将需要长达24小时才能显示加法。</span><span class="sxs-lookup"><span data-stu-id="f4629-132">When adding an attribute to profile card, it takes up to 24 hours for the addition to be displayed.</span></span>

## <a name="example"></a><span data-ttu-id="f4629-133">示例</span><span class="sxs-lookup"><span data-stu-id="f4629-133">Example</span></span>

<span data-ttu-id="f4629-134">下面的示例显示 `Alias` 配置文件卡片上的属性：</span><span class="sxs-lookup"><span data-stu-id="f4629-134">The following example displays the `Alias` attribute on the profile card:</span></span>

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

<span data-ttu-id="f4629-135">如果成功，响应会 `201 OK` 在响应正文中返回响应代码和**profileCardProperty**对象。</span><span class="sxs-lookup"><span data-stu-id="f4629-135">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="f4629-136">属性的值 `Alias` 将显示在用户的配置文件卡片上。</span><span class="sxs-lookup"><span data-stu-id="f4629-136">The value for the `Alias` attribute  would be displayed on a user's profile card.</span></span>  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a><span data-ttu-id="f4629-137">添加自定义属性</span><span class="sxs-lookup"><span data-stu-id="f4629-137">Adding custom attributes</span></span>

<span data-ttu-id="f4629-138">您可以通过配置组织设置并在 Microsoft Graph 中[将相应的值添加为 profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) ，将任何15个 Azure AD[自定义扩展属性](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)添加到用户的配置文件卡中。</span><span class="sxs-lookup"><span data-stu-id="f4629-138">You can add any of the 15 Azure AD [custom extension attributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) to users' profile cards by configuring your organization settings and [adding the corresponding value as a profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) in Microsoft Graph.</span></span> <span data-ttu-id="f4629-139">您可以一次添加一个**profileCardProperty**资源。</span><span class="sxs-lookup"><span data-stu-id="f4629-139">You can add one **profileCardProperty** resource at a time.</span></span>

<span data-ttu-id="f4629-140">需要长达24小时才能在配置文件卡片上显示所做的更改。</span><span class="sxs-lookup"><span data-stu-id="f4629-140">It takes up to 24 hours for the changes to show on profile cards.</span></span>

<span data-ttu-id="f4629-141">自定义属性不可搜索，且不能用于在 Microsoft 应用程序和服务中搜索人员。</span><span class="sxs-lookup"><span data-stu-id="f4629-141">Custom properties are not searchable and can't be used to search for people across Microsoft apps and services.</span></span>

<span data-ttu-id="f4629-142">下表显示了 Azure AD 自定义扩展属性名称如何对应于[profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta)资源的**directoryPropertyName**属性的受支持的值。</span><span class="sxs-lookup"><span data-stu-id="f4629-142">The following table shows how the Azure AD custom extension attribute names correspond to the supported values for the **directoryPropertyName** property of the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource.</span></span> <span data-ttu-id="f4629-143">这些 Azure AD 自定义扩展属性名称*不区分大小写*：</span><span class="sxs-lookup"><span data-stu-id="f4629-143">These Azure AD custom extension attribute names are *not case-sensitive*:</span></span>

|<span data-ttu-id="f4629-144">Azure AD 自定义扩展属性</span><span class="sxs-lookup"><span data-stu-id="f4629-144">Azure AD custom extension attribute</span></span> | <span data-ttu-id="f4629-145">要指定为 directoryPropertyName 的值</span><span class="sxs-lookup"><span data-stu-id="f4629-145">Value to specify as directoryPropertyName</span></span> |
|:--------------------|:-----------------|
| <span data-ttu-id="f4629-146">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="f4629-146">extensionAttribute1</span></span> | <span data-ttu-id="f4629-147">customAttribute1</span><span class="sxs-lookup"><span data-stu-id="f4629-147">customAttribute1</span></span> |
| <span data-ttu-id="f4629-148">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="f4629-148">extensionAttribute2</span></span> | <span data-ttu-id="f4629-149">customAttribute2</span><span class="sxs-lookup"><span data-stu-id="f4629-149">customAttribute2</span></span> |
| <span data-ttu-id="f4629-150">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="f4629-150">extensionAttribute3</span></span> | <span data-ttu-id="f4629-151">customAttribute3</span><span class="sxs-lookup"><span data-stu-id="f4629-151">customAttribute3</span></span> |
| <span data-ttu-id="f4629-152">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="f4629-152">extensionAttribute4</span></span> | <span data-ttu-id="f4629-153">customAttribute4</span><span class="sxs-lookup"><span data-stu-id="f4629-153">customAttribute4</span></span> |
| <span data-ttu-id="f4629-154">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="f4629-154">extensionAttribute5</span></span> | <span data-ttu-id="f4629-155">customAttribute5</span><span class="sxs-lookup"><span data-stu-id="f4629-155">customAttribute5</span></span> |
| <span data-ttu-id="f4629-156">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="f4629-156">extensionAttribute6</span></span> | <span data-ttu-id="f4629-157">customAttribute6</span><span class="sxs-lookup"><span data-stu-id="f4629-157">customAttribute6</span></span> |
| <span data-ttu-id="f4629-158">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="f4629-158">extensionAttribute7</span></span> | <span data-ttu-id="f4629-159">customAttribute7</span><span class="sxs-lookup"><span data-stu-id="f4629-159">customAttribute7</span></span> |
| <span data-ttu-id="f4629-160">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="f4629-160">extensionAttribute8</span></span> | <span data-ttu-id="f4629-161">customAttribute8</span><span class="sxs-lookup"><span data-stu-id="f4629-161">customAttribute8</span></span> |
| <span data-ttu-id="f4629-162">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="f4629-162">extensionAttribute9</span></span> | <span data-ttu-id="f4629-163">customAttribute9</span><span class="sxs-lookup"><span data-stu-id="f4629-163">customAttribute9</span></span> |
| <span data-ttu-id="f4629-164">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="f4629-164">extensionAttribute10</span></span> | <span data-ttu-id="f4629-165">customAttribute10</span><span class="sxs-lookup"><span data-stu-id="f4629-165">customAttribute10</span></span> |
| <span data-ttu-id="f4629-166">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="f4629-166">extensionAttribute11</span></span> | <span data-ttu-id="f4629-167">customAttribute11</span><span class="sxs-lookup"><span data-stu-id="f4629-167">customAttribute11</span></span> |
| <span data-ttu-id="f4629-168">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="f4629-168">extensionAttribute12</span></span> | <span data-ttu-id="f4629-169">customAttribute12</span><span class="sxs-lookup"><span data-stu-id="f4629-169">customAttribute12</span></span> |
| <span data-ttu-id="f4629-170">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="f4629-170">extensionAttribute13</span></span> | <span data-ttu-id="f4629-171">customAttribute13</span><span class="sxs-lookup"><span data-stu-id="f4629-171">customAttribute13</span></span> |
| <span data-ttu-id="f4629-172">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="f4629-172">extensionAttribute14</span></span> | <span data-ttu-id="f4629-173">customAttribute14</span><span class="sxs-lookup"><span data-stu-id="f4629-173">customAttribute14</span></span> |
| <span data-ttu-id="f4629-174">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="f4629-174">extensionAttribute15</span></span> | <span data-ttu-id="f4629-175">customAttribute15</span><span class="sxs-lookup"><span data-stu-id="f4629-175">customAttribute15</span></span> |

## <a name="example"></a><span data-ttu-id="f4629-176">示例</span><span class="sxs-lookup"><span data-stu-id="f4629-176">Example</span></span>

<span data-ttu-id="f4629-177">下面的示例使用显示名称**成本中心**将第一个 Azure AD 自定义扩展属性添加到配置文件卡片中。</span><span class="sxs-lookup"><span data-stu-id="f4629-177">The following example adds the first Azure AD custom extension attribute to the profile card, using the display name **Cost center**.</span></span> <span data-ttu-id="f4629-178">对于已将其语言设置设置为德语的用户，显示名称将为**Kostenstelle**。</span><span class="sxs-lookup"><span data-stu-id="f4629-178">For users that have set their language settings to German, the display name will be **Kostenstelle**.</span></span>

```http
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

<span data-ttu-id="f4629-179">如果语言不受支持，则将以默认值显示属性名称。</span><span class="sxs-lookup"><span data-stu-id="f4629-179">If a language is not supported, the property name will be shown with the default value.</span></span>  

<span data-ttu-id="f4629-180">如果成功，响应会 `201 OK` 在响应正文中返回响应代码和**profileCardProperty**对象。</span><span class="sxs-lookup"><span data-stu-id="f4629-180">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="f4629-181">在此示例中，您可以假定配置文件卡片显示了在配置文件卡片上将其语言设置为德语的所有用户的**Kostenstelle** 。</span><span class="sxs-lookup"><span data-stu-id="f4629-181">In this example you can assume that the profile card displays **Kostenstelle** for all users that have set their language settings to German on the profile card.</span></span> <span data-ttu-id="f4629-182">对于所有其他用户，**成本中心**将显示在配置文件卡片上。</span><span class="sxs-lookup"><span data-stu-id="f4629-182">For all other users, **Cost center** will be displayed on the profile card.</span></span>

```http
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

## <a name="see-also"></a><span data-ttu-id="f4629-183">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f4629-183">See also</span></span>

[<span data-ttu-id="f4629-184">查找你的 Microsoft 365 租户 ID</span><span class="sxs-lookup"><span data-stu-id="f4629-184">Find your Microsoft 365 tenant ID</span></span>](https://docs.microsoft.com/onedrive/find-your-office-365-tenant-id)

[<span data-ttu-id="f4629-185">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4629-185">onPremisesExtensionAttributes resource type</span></span>](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[<span data-ttu-id="f4629-186">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="f4629-186">User resource type</span></span>](/graph/api/resources/user?view=graph-rest-beta)

[<span data-ttu-id="f4629-187">Graph 浏览器</span><span class="sxs-lookup"><span data-stu-id="f4629-187">Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)

[<span data-ttu-id="f4629-188">获取 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="f4629-188">Get profileCardProperty</span></span>](/graph/api/profilecardproperty-get?view=graph-rest-beta)
