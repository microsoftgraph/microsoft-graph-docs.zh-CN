# <a name="passwordprofile-resource-type"></a><span data-ttu-id="94376-101">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="94376-101">passwordProfile resource type</span></span>

<span data-ttu-id="94376-p101">包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="94376-p101">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="94376-104">属性</span><span class="sxs-lookup"><span data-stu-id="94376-104">Properties</span></span>
| <span data-ttu-id="94376-105">属性</span><span class="sxs-lookup"><span data-stu-id="94376-105">Property</span></span>     | <span data-ttu-id="94376-106">类型</span><span class="sxs-lookup"><span data-stu-id="94376-106">Type</span></span>   |<span data-ttu-id="94376-107">说明</span><span class="sxs-lookup"><span data-stu-id="94376-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94376-108">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="94376-108">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="94376-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="94376-109">Boolean</span></span>| <span data-ttu-id="94376-110">如果用户在下次登录时必须更改密码，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="94376-110">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="94376-111">密码</span><span class="sxs-lookup"><span data-stu-id="94376-111">password</span></span>|<span data-ttu-id="94376-112">String</span><span class="sxs-lookup"><span data-stu-id="94376-112">String</span></span>|<span data-ttu-id="94376-p102">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="94376-p102">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94376-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94376-118">JSON representation</span></span>

<span data-ttu-id="94376-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94376-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->