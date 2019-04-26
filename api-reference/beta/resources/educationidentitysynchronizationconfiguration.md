    ---
<span data-ttu-id="baa73-101">标题: "educationIdentitySynchronizationConfiguration 资源类型" 说明: "所有学校数据配置文件标识同步配置的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="baa73-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="baa73-102">派生类定义用于同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="baa73-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="baa73-103">以下是派生类型。</span><span class="sxs-lookup"><span data-stu-id="baa73-103">The following are the derived types."</span></span>
<span data-ttu-id="baa73-104">author: "mmast-msft" 使用: 正常毫秒: "教育版"</span><span class="sxs-lookup"><span data-stu-id="baa73-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="baa73-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="baa73-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baa73-106">所有学校数据配置文件标识同步配置的摘要基类。</span><span class="sxs-lookup"><span data-stu-id="baa73-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="baa73-107">派生类定义用于同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="baa73-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="baa73-108">以下是派生类型。</span><span class="sxs-lookup"><span data-stu-id="baa73-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="baa73-109">派生类型</span><span class="sxs-lookup"><span data-stu-id="baa73-109">Derived types</span></span>
| <span data-ttu-id="baa73-110">类型</span><span class="sxs-lookup"><span data-stu-id="baa73-110">Type</span></span> | <span data-ttu-id="baa73-111">说明</span><span class="sxs-lookup"><span data-stu-id="baa73-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="baa73-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="baa73-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="baa73-113">使用此类型可匹配 azure Active Directory (azure AD) 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="baa73-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="baa73-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="baa73-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="baa73-115">使用此类型在 Azure AD 中创建新用户帐户。</span><span class="sxs-lookup"><span data-stu-id="baa73-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="baa73-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baa73-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

