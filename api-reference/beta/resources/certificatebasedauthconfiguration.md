---
title: certificateBasedAuthConfiguration 资源类型
description: 表示证书颁发机构的集合。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76178d8d70225a8cf861f5ff5e1cdaf7f0f69f60
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667627"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="e0b60-103">certificateBasedAuthConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0b60-103">certificateBasedAuthConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0b60-104">通过基于证书的身份验证, 您可以在将 Exchange Online 帐户连接到以下各项时, 使用 Windows、Android 或 iOS 设备上的客户端证书对 Azure Active Directory 进行身份验证:</span><span class="sxs-lookup"><span data-stu-id="e0b60-104">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="e0b60-105">Microsoft 移动应用程序 (如 Outlook 和 Word)</span><span class="sxs-lookup"><span data-stu-id="e0b60-105">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="e0b60-106">Exchange ActiveSync (EAS) 客户端</span><span class="sxs-lookup"><span data-stu-id="e0b60-106">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="e0b60-107">配置此功能后, 无需在移动设备上将用户名和密码组合输入到某些邮件和 Microsoft Office 应用程序中。</span><span class="sxs-lookup"><span data-stu-id="e0b60-107">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="e0b60-108">基于证书的身份验证配置是通过证书颁发机构的集合提供的。</span><span class="sxs-lookup"><span data-stu-id="e0b60-108">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="e0b60-109">证书颁发机构用于建立受信任的证书链, 使客户端能够通过具有客户端证书的 Azure Active Directory 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e0b60-109">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="e0b60-110">了解有关[Azure Active Directory 中基于证书的身份验证的](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)详细信息。</span><span class="sxs-lookup"><span data-stu-id="e0b60-110">Learn more about [certificate-based authentication in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="e0b60-111">方法</span><span class="sxs-lookup"><span data-stu-id="e0b60-111">Methods</span></span>

| <span data-ttu-id="e0b60-112">方法</span><span class="sxs-lookup"><span data-stu-id="e0b60-112">Method</span></span>       | <span data-ttu-id="e0b60-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0b60-113">Return Type</span></span> | <span data-ttu-id="e0b60-114">说明</span><span class="sxs-lookup"><span data-stu-id="e0b60-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e0b60-115">列出 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0b60-115">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="e0b60-116">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0b60-116">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="e0b60-117">列出**certificateBasedAuthConfiguration**集合的属性。</span><span class="sxs-lookup"><span data-stu-id="e0b60-117">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="e0b60-118">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0b60-118">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="e0b60-119">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0b60-119">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="e0b60-120">读取**certificateBasedAuthConfiguration**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0b60-120">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="e0b60-121">创建 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0b60-121">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="e0b60-122">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0b60-122">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="e0b60-123">创建新的**certificateBasedAuthConfiguration**对象。</span><span class="sxs-lookup"><span data-stu-id="e0b60-123">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="e0b60-124">删除 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0b60-124">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="e0b60-125">无</span><span class="sxs-lookup"><span data-stu-id="e0b60-125">None</span></span> | <span data-ttu-id="e0b60-126">删除**certificateBasedAuthConfiguration**对象。</span><span class="sxs-lookup"><span data-stu-id="e0b60-126">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="e0b60-127">不支持更新 cerficateBasedAuthConfiguration。</span><span class="sxs-lookup"><span data-stu-id="e0b60-127">Updating cerficateBasedAuthConfiguration is not supported.</span></span> <span data-ttu-id="e0b60-128">若要更改 cerficateBasedAuthConfiguration, 请先删除, 然后创建一个新的 cerficateBasedAuthConfiguration。</span><span class="sxs-lookup"><span data-stu-id="e0b60-128">To change a cerficateBasedAuthConfiguration, first delete and then create a new cerficateBasedAuthConfiguration.</span></span>

## <a name="properties"></a><span data-ttu-id="e0b60-129">属性</span><span class="sxs-lookup"><span data-stu-id="e0b60-129">Properties</span></span>

| <span data-ttu-id="e0b60-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0b60-130">Property</span></span>     | <span data-ttu-id="e0b60-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0b60-131">Type</span></span>        | <span data-ttu-id="e0b60-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0b60-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0b60-133">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="e0b60-133">certificateAuthorities</span></span>|<span data-ttu-id="e0b60-134">[certificateAuthority](certificateauthority.md)集合</span><span class="sxs-lookup"><span data-stu-id="e0b60-134">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="e0b60-135">创建受信任的证书链的证书颁发机构的集合。</span><span class="sxs-lookup"><span data-stu-id="e0b60-135">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="e0b60-136">id</span><span class="sxs-lookup"><span data-stu-id="e0b60-136">id</span></span>|<span data-ttu-id="e0b60-137">String</span><span class="sxs-lookup"><span data-stu-id="e0b60-137">String</span></span>|<span data-ttu-id="e0b60-138">基于证书的身份验证配置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e0b60-138">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="e0b60-139">只读。</span><span class="sxs-lookup"><span data-stu-id="e0b60-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0b60-140">关系</span><span class="sxs-lookup"><span data-stu-id="e0b60-140">Relationships</span></span>

<span data-ttu-id="e0b60-141">无</span><span class="sxs-lookup"><span data-stu-id="e0b60-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0b60-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0b60-142">JSON representation</span></span>

<span data-ttu-id="e0b60-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0b60-143">The following is a JSON representation of the resource.</span></span>

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
