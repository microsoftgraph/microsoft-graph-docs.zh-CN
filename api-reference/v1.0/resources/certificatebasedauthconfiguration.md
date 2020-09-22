---
title: certificateBasedAuthConfiguration 资源类型
description: 表示证书颁发机构的集合。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 834ca029692bfcf3bcb6a65ab8a0d4b84ed0216a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037911"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="f8b08-103">certificateBasedAuthConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8b08-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="f8b08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8b08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8b08-105">通过基于证书的身份验证，您可以在将 Exchange Online 帐户连接到以下各项时，使用 Windows、Android 或 iOS 设备上的客户端证书对 Azure Active Directory 进行身份验证：</span><span class="sxs-lookup"><span data-stu-id="f8b08-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="f8b08-106">Microsoft 移动应用程序（如 Outlook 和 Word）</span><span class="sxs-lookup"><span data-stu-id="f8b08-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="f8b08-107">Exchange ActiveSync (EAS) 客户端</span><span class="sxs-lookup"><span data-stu-id="f8b08-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="f8b08-108">配置此功能后，无需在移动设备上将用户名和密码组合输入到某些邮件和 Microsoft Office 应用程序中。</span><span class="sxs-lookup"><span data-stu-id="f8b08-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="f8b08-109">基于证书的身份验证配置是通过证书颁发机构的集合提供的。</span><span class="sxs-lookup"><span data-stu-id="f8b08-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="f8b08-110">证书颁发机构用于建立受信任的证书链，使客户端能够通过具有客户端证书的 Azure Active Directory 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="f8b08-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="f8b08-111">了解有关 [Azure Active Directory 中基于证书的身份验证的](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)详细信息。</span><span class="sxs-lookup"><span data-stu-id="f8b08-111">Learn more about [certificate-based authentication in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="f8b08-112">方法</span><span class="sxs-lookup"><span data-stu-id="f8b08-112">Methods</span></span>

| <span data-ttu-id="f8b08-113">方法</span><span class="sxs-lookup"><span data-stu-id="f8b08-113">Method</span></span>       | <span data-ttu-id="f8b08-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8b08-114">Return Type</span></span> | <span data-ttu-id="f8b08-115">说明</span><span class="sxs-lookup"><span data-stu-id="f8b08-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f8b08-116">列出 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8b08-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="f8b08-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8b08-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="f8b08-118">列出 **certificateBasedAuthConfiguration** 集合的属性。</span><span class="sxs-lookup"><span data-stu-id="f8b08-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="f8b08-119">创建 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8b08-119">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="f8b08-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8b08-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="f8b08-121">创建新的 **certificateBasedAuthConfiguration** 对象。</span><span class="sxs-lookup"><span data-stu-id="f8b08-121">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="f8b08-122">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8b08-122">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="f8b08-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8b08-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="f8b08-124">读取 **certificateBasedAuthConfiguration** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f8b08-124">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="f8b08-125">删除 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8b08-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="f8b08-126">无</span><span class="sxs-lookup"><span data-stu-id="f8b08-126">None</span></span> | <span data-ttu-id="f8b08-127">删除 **certificateBasedAuthConfiguration** 对象。</span><span class="sxs-lookup"><span data-stu-id="f8b08-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="f8b08-128">不支持更新 **cerficateBasedAuthConfiguration** 。</span><span class="sxs-lookup"><span data-stu-id="f8b08-128">Updating **cerficateBasedAuthConfiguration** is not supported.</span></span> <span data-ttu-id="f8b08-129">若要更改 **cerficateBasedAuthConfiguration**，请先删除，然后创建一个新的 **cerficateBasedAuthConfiguration**。</span><span class="sxs-lookup"><span data-stu-id="f8b08-129">To change a **cerficateBasedAuthConfiguration**, first delete and then create a new **cerficateBasedAuthConfiguration**.</span></span>

## <a name="properties"></a><span data-ttu-id="f8b08-130">属性</span><span class="sxs-lookup"><span data-stu-id="f8b08-130">Properties</span></span>

| <span data-ttu-id="f8b08-131">属性</span><span class="sxs-lookup"><span data-stu-id="f8b08-131">Property</span></span>     | <span data-ttu-id="f8b08-132">类型</span><span class="sxs-lookup"><span data-stu-id="f8b08-132">Type</span></span>        | <span data-ttu-id="f8b08-133">说明</span><span class="sxs-lookup"><span data-stu-id="f8b08-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f8b08-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="f8b08-134">certificateAuthorities</span></span>|<span data-ttu-id="f8b08-135">[certificateAuthority](certificateauthority.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8b08-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="f8b08-136">创建受信任的证书链的证书颁发机构的集合。</span><span class="sxs-lookup"><span data-stu-id="f8b08-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="f8b08-137">id</span><span class="sxs-lookup"><span data-stu-id="f8b08-137">id</span></span>|<span data-ttu-id="f8b08-138">String</span><span class="sxs-lookup"><span data-stu-id="f8b08-138">String</span></span>|<span data-ttu-id="f8b08-139">基于证书的身份验证配置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f8b08-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="f8b08-140">只读。</span><span class="sxs-lookup"><span data-stu-id="f8b08-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8b08-141">关系</span><span class="sxs-lookup"><span data-stu-id="f8b08-141">Relationships</span></span>

<span data-ttu-id="f8b08-142">无</span><span class="sxs-lookup"><span data-stu-id="f8b08-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8b08-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8b08-143">JSON representation</span></span>

<span data-ttu-id="f8b08-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8b08-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

