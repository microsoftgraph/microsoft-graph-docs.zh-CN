---
title: educationIdentityCreationConfiguration 资源类型
description: 创建学校数据配置文件标识上定义的设置。 这些身份包括学生和教师。 根据这些设置，将在目录中创建用户。
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048493"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="14555-105">educationIdentityCreationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="14555-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="14555-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="14555-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14555-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="14555-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14555-108">创建学校数据配置文件标识上定义的设置。</span><span class="sxs-lookup"><span data-stu-id="14555-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="14555-109">这些身份包括学生和教师。</span><span class="sxs-lookup"><span data-stu-id="14555-109">These identities include students and teachers.</span></span> <span data-ttu-id="14555-110">根据这些设置，将在目录中创建用户。</span><span class="sxs-lookup"><span data-stu-id="14555-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="14555-111">**注意：** 如果您有目录同步到本地之间的同步开启，Active Directory 和 Azure Active Directory (Azure AD)，请改用[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)资源。</span><span class="sxs-lookup"><span data-stu-id="14555-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="14555-112">派生自[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="14555-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="14555-113">属性</span><span class="sxs-lookup"><span data-stu-id="14555-113">Properties</span></span>

| <span data-ttu-id="14555-114">属性</span><span class="sxs-lookup"><span data-stu-id="14555-114">Property</span></span> | <span data-ttu-id="14555-115">类型</span><span class="sxs-lookup"><span data-stu-id="14555-115">Type</span></span> | <span data-ttu-id="14555-116">说明</span><span class="sxs-lookup"><span data-stu-id="14555-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="14555-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="14555-117">**userDomains**</span></span> | <span data-ttu-id="14555-118">[educationIdentityDomain](educationidentitydomain.md)集合</span><span class="sxs-lookup"><span data-stu-id="14555-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="14555-119">设置要使用的每个用户类型的域的列表。</span><span class="sxs-lookup"><span data-stu-id="14555-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="14555-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14555-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```